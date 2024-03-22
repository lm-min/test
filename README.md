
# CSS 규칙
#### 아래 순서로 적용시키면 됩니다.

- @include ~
- position
- display
- width
- height
- margin
- padding
- text - font
- color
- border
- background
- transition
- 기타 등등
- z-index (마지막)


`````````
.sample{

  @include keyframes;

  position: absolute;
  top: 0;

  display: flex;
  flex-direction: column;
  gap: 5px;

  width: 10%;
  height: 10%;

  text-wrap: nowrap;
  letter-spacing: -1px;

  font-size: 14px;
  font-weight: bold;

  color: red;

  border: 1px solid red;
  border-radius: 50%;

  background: red;

  box-shadow: red;

  transition: all .3s;

  <!-- To. 규칙 외 css code.  -->
  opacity: 0;
  visibility: hidden;
  transform: rotate(12deg);

  <!-- To. z-index 마지막에 적용합니다.  -->
  z-index: 999; 

}

`````````
