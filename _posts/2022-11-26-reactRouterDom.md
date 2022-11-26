---
layout: single
title: "Object Literal"
---

# React Router Dom

```sh
npm i react-router-dom
```

npm을 이용한 설치 명령어



```react
import BrowserRouter from 'react-router-dom'
```

BrowserRouter를 import해준 뒤

```react
<BrowserRouter>
  <App />
</BrowserRouter>
```

BrowserRouter는 HTML5 history API를 이용하여 UI를 URL과 동기화 시켜주는 기능을 한다. (pushState, replaceState, popstate)

react-router-dom을 사용하여 라우팅 시에  최상단에 위치하여야 한다.