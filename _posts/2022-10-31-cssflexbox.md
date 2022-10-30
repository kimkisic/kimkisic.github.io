---
layout : single
title : "CSS Flexbox"
---



# CSS Flexbox

행과 열 형태로 항목 무리를 배치하는 일차원 레이아웃 메서드

하나의 컨테이너에서 콘텐츠들의 동일한 사이즈 정렬이나,

콘텐츠의 중심부정렬 같은 작업들에 대해 편하게 작업하도록 만들어준다.



## The flex model

![img](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox/flex_terms.png)

- `main axis` 은 flex item이 배치되고 있는 방향으로 진행하는 축이며,

  축의 시작과 끝을 일컬어 **main start**과 **main end**라고 합니다.

- `cross axis`은 flex item이 내부에 배치되는 방향에 직각을 이루는 축이며,

  이 축의 시작과 끝을 일컬어 **cross start**과 **cross end**라고 합니다.

  

### Columns or rows?

flexbox는 main axis가 진행되는 방향을 지정하는 flex-direction속성을 제공하는데

기본값은 row로 설정되어 설정값이 없으면 왼쪽에서 오른쪽으로 배치된다.

```css
flex-direction: column;
```

위 코드를 통해 flex-direction속성을 column으로 변경하면 위에서 아래로 배치된다.

```css
flex-direction: row-reverse;
flex-direction: column-reverse;
```

row속성과 column속성 외에 row-reverse속성과 column-reverse속성을 통해

기존 속성과 반대로 오른쪽에서 왼쪽으로, 아래에서 위로 배치되도록 가능하다.



##### justify-content

```css
/* Positional alignment */
justify-content: center;     /* Pack items around the center */
justify-content: start;      /* Pack items from the start */
justify-content: end;        /* Pack items from the end */
justify-content: flex-start; /* Pack flex items from the start */
justify-content: flex-end;   /* Pack flex items from the end */
justify-content: left;       /* Pack items from the left */
justify-content: right;      /* Pack items from the right */

/* Distributed alignment */
justify-content: space-between; /* Distribute items evenly
                                   The first item is flush with the start,
                                   the last is flush with the end */
justify-content: space-around;  /* Distribute items evenly
                                   Items have a half-size space
                                   on either end */
justify-content: space-evenly;  /* Distribute items evenly
                                   Items have equal space around them */
```

space-between : 첫번째 콘텐츠와 마지막 콘텐츠는 간격없이.

space-around : 첫번째 콘텐츠와 마지막 콘텐츠는 간격의 반만큼.

space-evenly : 모든 간격이 동일하게.