# Overwatch hero selector example

지금까지 학습한 HTML/CSS 를 활용해서 오버워치 영웅 선택 화면을 만들어보았습니다.

학습하면서 기억하고 싶은 내용을 정리해볼게요
<br><br><br>
> ### 한번에 같은 코드를 반복으로 작성하고 싶을 때
```
<div class="hero">
  <div class="image"></div>
</div>
```

위와 같은 코드를 반복적으로 입력하고 싶을 때 복붙을 계속 하는건 너무 지쳐... <b>No NO!!!!</b>

이럴 땐 아래와 같이 코드를 입력하고 `tab` 키를 눌러주면 같은 코드 32번을 한번에 자동완성 할 수 있다!!

`.hero*32>.image`

이건 hero 라는 클래스명의 div를 32개 만들건데 그 요소는 자식으로 image 라는 클래스명의 div를 가지고 있습니다. 라는 뜻!

알고보면 간단하지만 모르던 사람에겐 꿀팁~~! 다음에 꼭 다시 한번 사용해보겠어요!

<br><br>

> ### margin 과 padding 을 좀 더 깔끔하게 쓰는 방법
예전엔 margin 과 padding을 떡칠해서 어째저째 정렬을 맞추곤 했지만, 이젠 container를 만들고 그것에 margin 과 padding 을 부여해서 정렬할 수 있게 되었다!
```
max-width: 660px;
margin: 0 auto;
padding: 40px 20px;
```
최대 가로 너비를 주고 그 이상 커졌을 땐 남은 여백에서 정렬하기 위해 `margin: 0 auto`를 적용해서 좌우 정렬을 맞춰준다.

<br><br>

> ### `transform : skew 함수`
부모 요소에 skew 함수를 써서 기울이면 자식 요소도 같이 기울어지므로 자식 요소를 원래대로 보여주고 싶다면 자식 요소에 다시 skew 함수를 이용해서 반대로 값을 넣어주면 원상태로 보일 수 있다.

```
/* 부모 요소에 적용한 skew 함수 */
transform: skewX(-14deg);

/* 자식 요소에 적용한 skew 함수 */
transform: skewX(14deg);
```

<br><br>

> ### transition 속성
```
transition:
  transform .1s,
  background-color .6s;
```
각 속성에 따라 지속시간 다르게 줄 수 있는 걸 알고는 있었지만 실제로 적용해보니 신기하다 🤭

<br>

### 다음 번엔 더 멋진 페이지로 돌아올게요~!! 😶‍🌫️💜
