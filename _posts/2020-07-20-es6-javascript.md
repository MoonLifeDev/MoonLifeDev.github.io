---
layout: post
title: Javascript ES6 Class extends 간략한 활용
category: ES6
tags: [ES6]
comments: true
---

> Javascript ES6 Class extends 간략한 활용<br>
> 조금 더 구체적인 설명은 => [드림코딩 엘리](https://www.youtube.com/watch?v=_DLhUBWsRtw)를 확인하세요!<br>

## Class의 extends(상속과 다양성)은..!

>만약 우리가 좋아하는 아이스크림 붕어 싸만코를 초코, 바닐라, 딸기처럼 맛 별로 __구별하고자 할 때(다양성)__ <br>
>붕어 싸만코의 __공통적인 요소를(상속)__ 할 수 있게 탬플릿(template)를 만들고<br>
>flavor만 첨가해 준다 생각하면 이해하기 쉽다.

```javascript
" use strict ";

class SaManKo {
    construtor(flavor, width, height){
        this.flavor = flavor;
        this.width = width;
        this.height = height;
    }
    getFlavor(){
        console.log`This Samanko taste like ${flavor}`
    }
    getSize(){
        return this.width * this.height / 2 ;
    }
}

class ChocoManKo extends SaManKo {
    getFlavor(){
        super.getFlavor();
    }
    getSize(){
        super.getSize();
    }
}
// 초코 싸만코 만들기
const chocoTaste = new ChocoManKo("choco", 20, 20);
chocoTaste.getFlavor();
console.log(chocoTaste.getSize());
```

__기존의 싸만코 틀에서 초코 싸만코를 만들어 보았다.__