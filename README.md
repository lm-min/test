
# SCSS 선언순서 및 규칙



>아래 순서대로하면 됩니다.
  1. @include
  2. content
  3. position / float / transform
  4. display
  5. width/height
  6. margin / padding
  7. color / text / font
  8. border
  9. background
  10. box-shadow
  11. transition
  12. 그 외의 기타 css code ( animation, opacity, visibility ··· )
  13. z-index


⚠️@include 사용하더라도 media 경우 최하단에 선언.

****

>예시
`````````
.sample{

  @include keyframes;

  position: absolute;
  top: 0;
  transform: translateY(-50%) rotate(12deg);

  display: flex;
  flex-direction: column;
  gap: 5px;

  width: 10%;
  height: 10%;

  color: red;
  text-wrap: nowrap;
  letter-spacing: -1px;
  font-size: 14px;
  font-weight: bold;

  border: 1px solid red;
  border-radius: 50%;

  background: url('/images/img.png') no-repeat center left/18px auto;

  box-shadow: red;

  transition: all .3s;

  animation: ani 3s linear infinite;
  opacity: 0;
  visibility: hidden;
  
  z-index: 999; 
}

`````````
