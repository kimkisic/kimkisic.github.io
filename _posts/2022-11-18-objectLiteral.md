---
layout: single
title: "Object Literal"
---

# 객체 리터럴

```javascript
// new키워드를 이용한 객체 생성방법
const obj = new Object();
obj.name = 'kim';
obj.age = 27;
console.log(obj); // { name: 'kim', age: 27 }

// 객체리터럴을 이용한 객체 생성방법
const objLit = {};
objLit.name = 'lee';
objLit.age = 21;
console.log(objLit); // { name: 'lee', age: 21 }
```

정확히 동일한 작동을 하지만,

가독성, 단순성 및 실행속도를 위해 객체 리터럴 방법을 사용

