# CSS

# 1. CSS 선택자

## 1.1 전체 선택자

- universal.html

## 1.2 태그 선택자

- tag.html

## 1.3 자손 선택자

- descendant.html

## 1.4 자식 선택자

- child.html

## 1.5 그룹 선택자

- group.html

## 1.6 순서 선택자

- order.html

## 1.7 속성 선택자

- properties.html

## 1.8 가상 선택자

- pesudo.html

# 2. 폰트 스타일링

## 2.1 font-weight

- 폰트 굵기
- bold, normal

## 2.2 font-size

### 2.2.1 px

- 폰트 크기 픽셀 단위

### 2.2.2 rem

- root em 최상위 부모 html 태그를 기준으로 폰트 크기 설정
- 많이 사용하는 단위

### 2.2.3 em

- 부모 요소를 기준으로 폰트크기 설정

## 2.3 font-family 글꼴

- [구글폰트](https://fonts.google.com/)
- [눈누](https://noonnu.cc/)

## 2.4 딩벳폰트

- [폰트어썸](https://fontawesome.com/)

## 2.5 color 폰트 색상

- 영문명, 15진수 표기, RGB

## 2.6 line-height 행간

- 픽셀값 : 줄 간격을 고정된 px 단위로 지정
- 실숫값 : 줄 간격을 폰트 크기에 맞춰 실수 배율로 지정

## 2.7 letter-spacing 자간

- 픽셀

# 3. 영역 크기

## 3.1 width, height

### 3.1.1 width-height.html

- px : 너빗값, 높이값 px 단위로 지정
- % : 부모 태그 기준
- vw : 웹 브라우저의 너비를 기준으로 백분율 너비, 높이 지정
- vh : 웹 브라우저의 너비를 기준으로 백분율 너비, 높이 지정

### 3.1.2 max-width, max-height

## 3.2 margin, padding

- margin-top > margin-right > margin-bottom > margin-left
- padding-top > padding-right > padding-bottom > padding-left

### 3.2.1. margin-top 중첩현상

- margin-top과 magin-bottom 중에 크기가 큰 것이 적용됨 (큰놈이 잡아먹는다)

## 3.3 border 테두리

- border-width : px, 테두리 굵기
- border-style : solid, dashed, dotted 테두리 모양
- border-color : 색상명, 16진수, rgb 테두리 색상
- border : width style color 테두리 굵기, 모양, 색상

## 3.4 블록 요소, 인라인 요소

### 3.4.1 블록 요소

- h1~h6, p, ol, ul, div, header, footer, section, article, aside, nav

### 3.4.2 인라인 요소

- strong, a, span
- display: inline-block

# 4. 배경

## 4.1 background-color 배경색 지정하기

- 색상명, 16진수, rgb

## 4.2 배경 이미지 삽입

- background-image : url(이미지 경로) 배경 이미지 삽입
- background-repeat : repeat, repeat-x, repeat-y, no-repeat 이미지 반복
- background-position : 가로축, 세로축
- background-size : contain, cover
- background-attachment : fixed 고정

# 5. 레이아웃

## 5.1 CSS 초기화

- 크로스 브라우징 normalize.css, reset.css
- 사용자 초기화 global.css

## 5.2 float - 블록 요소 좌우로 배치

- float : left, 왼쪽부터 차례대로
- float : right, 오른쪽부터 차례대로
- clear : both, left, right

# 6. 그래픽 효과

## 6.1 box-shadow, text-shadow 요소의 그림자

- box-shadow: (inset) 가로축 세로축 퍼짐정도 색상 (블록 요소의 그림자)
- text-shadow: 가로축 세로축 퍼짐정도 색상 (텍스트의 그림자)

## 6.2 border-radious 모서리 둥글게

- border-radious: px, %

## 6.3 gradient

- linear-gradient (방향, 색상1, 색상2)
- radial-gradient (색상1, 색상2)

# 7. 인터랙티브 웹 CSS

## 7.1 변형하기

### 7.1.1 transform

- transform2d.html
- transform3d1.html
- transform3d2.html

#### 7.1.1.1 2D

- scale : 1보다 크면 확대, 작으면 축소
- skew : X축, Y축 비틀기 원하는 각도 지정하여 기울기 조정
- translate : X축, Y축 이동
- rotate : 원하는 각도 회전

#### 7.1.1.2 3D

- rotateX, rotateY
- translateZ

#### 7.1.1.3 그 외...

- perspective : px, 3D효과가 적용된 요소가 입체감 있게 보이도록 함
  속성값이 작을수록 3D요소의 왜곡이 심하게 나타나고 값이 클수록 완만해짐
- transform-style : preserve-3d, 3D효과 유지
- transform-origin : 가로축, 세로축, 요소의 중심축 변경

## 7.2 전환효과

### 7.2.1 transition-property: 속성명

- 전환 효과를 줄 CSS 속성명을 지정, 여러개 지정 가능, all 전체 속성

### 7.2.2 transition-duration: 지속 시간(초 단위)

- 전환 효과 지속할 시간 (0.5s, 1s)

### 7.2.3 transition-delay: 지연 시간(초 단위)

### 7.2.4 transition-timing-function: 가속도

- linear : 등속
- ease : 가속
- ease-in: 모션 시작 시 가속
- ease-out: 모션 종료 시 가속
- ease-in-out: 모션시작, 종료 시 모두 가속
- cubic-bezier: 사용자가 지정한 가속 효과

### 7.2.5 transition: 속성명 전환시간

## 7.3 자동으로 움직이는 애니메이션 효과 만들기

- animation.html
- transition 속성은 사용자의 특정 동작에 반응하는 모션기법
- 사용자가 어떤 동작을 하지 않아도 미리 지정한 조건에 맞게 자동으로 반복하는 애니메이션 효과

### 7.3.1 @keyframes

- 애니메이션 세트 지정
- 애니메이션 시작과 끝을 등록하여 사용자 모션을 등록한다.
- 0% (from) 는 시작점, 100% (to) 끝 지점을 의미, 중간 지점은 여러개 추가 가능

### 7.3.2 animation-name

- 이름
- 키프레임으로 등록한 모션의 이름을 호출

### 7.3.3 animation-duration

- 지속시간 (초 단위)
- 키프레임 모션 한 세트를 얼마 동안 동작하게 할지 등록

### 7.3.4 animation-timing-function

- 가속도

### 7.3.5 animation-iteration-count

- 반복 횟수
- infinite

### 7.3.6 animation-delay

- 지연 시간(초 단위)

### 7.3.7 animation-play-state

- running / paused

### 7.3.8 animation

- 이름 / 진행 시간 / 가속도 / 지연 시간 / 반복 횟수

## 7.4 화면 너비에 따라 웹 페이지 레이아웃 변경

- responsive.html
- 반응형 웹
- breakpoint
- 미디어 쿼리 이용
- @media screen and (max-width: 1000px){}

## 7.5 요소의 여백 비율 지정하기

- flex-grow 요소의 안쪽 여백 확대
  - 요소의 크기를 키웠을때 요소 안쪽 여백이 확대되는 비율 지정
- flex-shrink 요소의 안쪽 여백 축소
- flex-basis
- flex: flex-grow flex-shrink flex-basis;
