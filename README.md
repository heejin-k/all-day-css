# 빔캠프 종찬님의 CSS 특강

## 22.04.25 day 1

<details>
<summary><b>1. margin-auto</b></summary>
<div markdown="1">

- top, bottom, right, left 와 함꼐 사용하기

  - `right : 0 , left : 0`을 하면 요소가 차지하는 공간이 좌우로 쭉 늘어난다.
  - `bottom : 0 , top : 0` 역시 위 아래로 쭉 늘어난다.
  - 네가지를 전부 해주면 요소가 부모요소 전체를 차지하게 되는데, 여기서 `margin : auto`를 주게되면 가운데 정렬이 된다.

- flex와 함꼐 사용하기
  - flex로 가운데 정렬 한 상태에서 `margin-top : auto , margin-bottom : auto`을 주게 되면 사용 가능한 공간이 해당 요소에게 할당되어진다.

![image](https://user-images.githubusercontent.com/54096506/165565045-c9a1ca76-6745-49b9-af5b-5646fc4a3278.png)

</details>

<details>
<summary><b>2. nagative-margins</b></summary>
<div markdown="1">

![image](https://user-images.githubusercontent.com/54096506/165561981-d2b22f44-c1cc-448b-aa6b-79e5f04bbd40.png)

왼쪽의 피카츄 이미지에 margin : -200px을 주었더니 부모요소를 뚫고 올라가 입체적으로 표현되었다.

</details>

<details>
<summary><b>3. position</b></summary>
<div markdown="1">

![image](https://user-images.githubusercontent.com/54096506/165566736-367befbd-9e4b-4b86-bbc0-b3d0078c765c.png)

- absolute(보통 자식에게 준다)와 relative(부모)를 사용하여 요소의 위치를 조정할 수 있다.
- 꼭 absolute - relative 관계가 아니어도 가능하다 (ex absolute-absolute)
- 연결할 요소가 없으면 뷰포트가 기준이 된다.
</details>

---

## 22.04.28 day 2

<details>
<summary><b>과제 코드 리뷰 및 피드백</b></summary>
<div markdown="1">

- 반응형을 생각해서 만드는 것은 기본

- 최대한 비슷하게 만들어라
- list의 입력값이 많아졌을때 줄간격과 들여쓰기 유지해야할 것
- 마크업을 완료한 후 스타일링 하는 것이 아닌, 큰 틀을 먼저 마크업 + 스타일링 하기

</details>

<details>
<summary><b>CSS level up! tip</b></summary>
<div markdown="1">

- level up

  - 1단계 : 디자인 완벽하게 구현하기 
  - 2단계 : 입력값이 많아져도 디자인이 깨지지 않도록 만들기

  - 3단계 : 디테일, 유지보수, 확장성 고려한 CSS 스타일링

- 유연한 CSS 스타일링하기

  - wrap을 활용할것. (빨간색 틀이 wrap)
  - ![image](https://user-images.githubusercontent.com/54096506/166137342-c75be3a5-b47b-4423-85ec-88ef1ac69ed9.png)

  - 헤더와 메인, 푸터 등의 가운데 정렬은 공통 클래스인 wrap으로 조절한다
  - wrap은 고정값을주고, 안에 자식들은 wrap기준으로 퍼센트값을 넓이로 준다.
  - 반응형의 경우 wrap의 넓이만 고치면 끝!

</details>


-----
## 과제 구현 결과물

![image](https://user-images.githubusercontent.com/54096506/165576869-1aeb8de5-3199-47a8-b096-1b49e7359c31.png)

### 배운점

스터디에서 배운내용을 바로 적용시킬 수 있는 페이지라서 복습하는데 많은 도움이 됐다.

- 가상요소에 `position`, `top, bottom, left, right : 0` + `margin-auto` 사용하여 가운데 타임라인 줄에 활용하기!
- 가상요소 한번에 두개는 사용 불가능하다..!!
- 가상요소에 nth-child를 사용하고 싶을땐 nth-child먼저 적고 가상요소 적으면 가능하다.
- 특히 리스트의 블랙부분을 flex + margin-top-auto 사용하여 깔끔하게 딱 구현됐을때 너무 행복했다!!!!

### 페이지 링크

https://heejin-k.github.io/all-day-css/Day1/challenges/timeline/
