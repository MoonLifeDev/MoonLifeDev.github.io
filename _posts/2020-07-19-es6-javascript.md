---
layout: post
title: Javascript ES6 Class 간략한 활용
category: ES6
tags: [ES6]
comments: true
---

> Javascript ES6 Class 간략한 활용<br>
> 조금 더 구체적인 설명은 => [드림코딩 엘리](https://www.youtube.com/watch?v=_DLhUBWsRtw)를 확인하세요!<br>

## Class는 쉽게 말해 Template로 생각하자!

> 클라스를 쉽게 이해하자면 붕어빵을  만들기 위해 필요한 __제작틀(Template)__ 이라 생각하면 도움이 된다.<br>
> 그리고 그 틀에 적절한 __instance of object(재료)__ 을 넣음으로서 슈크림, 피자, 팥 등의 붕어빵들이 탄생하게 된다.<br>
> Class의 내부는 __fields와 methods__ 가 존재하고, 이들을 통해 __캡슐화__ 및 __상속과 다양성__이 발생한다.<br>

```javascript
" use strict ";

class FishBread {
  constructor(name, flavor) {
    this.name = name;
    this.flavor = flavor;
  }
  getBread() {
    console.log(`This is ${this.name}, and ${this.flavor}`);
  }
  getName() {
    return this.flavor;
  }
}

const fishBread = new FishBread("Red bean fish bread", "Red bean taste !");

fishBread.getBread();
```

__FishBread__ 의 붕어빵 제작틀을 통해 __field와 methods를 통해 redBeanFish를 추출__ 해 보았다.