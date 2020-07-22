---
layout: post
title: React styled-component 간략 활용
category: React
tags: [React]
comments: true
---

### Styled-component는 컴포넌트 생성과 스타일링을 간편하게 작성하게 도와준다.

- 컴포넌트 생성 및 외부 CSS로 스타일링 할 때

```javascript
/* CSS 파일 Import 해 준 모습 */
import css from "./css";

/* Component */
function MoonLife() {
  return <p>MoonLife</p>;
}

/* CSS */
p {
  color: tomato;
}
```

- 스타일 컴포넌트 활용 할 때

```javascript
/* Import Styled-components */
import styled from "styled-components";

/* useing Styled-components */
const MoonLife = styled.p`
  color: tomato;
`;
```

> styled뒤엔 사용할 html tag를 입력해 주면 된다.<br>
> ex ) const X = styled.html tag``;
