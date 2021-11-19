---
layout: post
title: "[오늘의 CSS] background-repeat 몰랐던 사실."
subtitle : 오늘의 CSS는 background-image와 관련된 속성 중 background-repeat의 몰랐던 기능을 알아본다.  
tags: [오늘의 CSS]
author: Sohyeon An
comments : True
---

오늘의 CSS는 background-image와 관련된 속성 중 background-repeat의 몰랐던 기능을 알아보겠다.  
출처는 바로 [여기](https://www.youtube.com/watch?v=IkVDgvnjCHo) 또는 아래 이미지를 클릭하면 영상을 시청 할 수 있다.

[![A CSS value you probably never knew about](https://www.youtube.com/watch?v=IkVDgvnjCHo/0.jpg)](https://www.youtube.com/watch?v=IkVDgvnjCHo)

[codepen 출처](https://codepen.io/kevinpowell/pen/oNgZPVK)

---

{% include codepen.html hash="yLoZvPP" title="background-repeat" %}

<br>

---
✔ 사실 `background-repeat`는 **shorthand** 였다는 사실!!!! 한 개 값 구문만 지정하면 두 개 값 구문의 단축 형태가 된다. 즉, `background-repeat: <repeat-x>, <repeat-y>`로 x축과 y축에 각각 다른 반복 방법을 적용할 수 있다.


- **space** : 이미지가 잘리지 않을 만큼 이미지를 반복한다. 제일 처음과 마지막 반복 이미지는 요소의 양쪽 끝에 고정되고, 각 이미지 사이에 남은 여백을 고르게 분배힌다.
- **round** : 가용 영역이 늘어나면 반복 이미지도 늘어나 여백을 남기지 않는다. 남은 공간이 이미지 너비의 절반 보다 클 경우에만 반복 횟수를 추가한다. 

<br>

더 자세한 내용은 [MDN](https://developer.mozilla.org/ko/docs/Web/CSS/background-repeat)에서 확인할 수 있다.

---
