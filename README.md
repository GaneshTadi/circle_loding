# circle_loding
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  display: flex;
  text-align: center;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.ring {
  position: absolute;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  animation: ring 2s linear infinite;
}

@keyframes ring {
  0%{
     transform:rotate(0deg);
     box-shadow: 1px 5px 3px #e65c00;
  }

  50%{
      transform:rotate(180deg);
      box-shadow: 1px 5px 3px #18b201;
  }

  80%{
       transform:rotate(288deg);
       box-shadow: 1px 5px 3px #0456c8;
  }
  100%{
    transform:rotate(360deg);
    box-shadow: 1px 5px 3px #e65c00;
  }
}

.ring:before {
  position: absolute;
  content: '';
  left: 0;
  top: 0;
  width: 100%;
  border-radius: 50%;
  box-shadow: 0 0 5px rgba(255, 255, 255, .3);
}

span {
  color: #737373;
  font-size: 20px;
  text-transform: uppercase;
  letter-spacing: 1px;
  line-height: 200px;
  animation: text 3s ease-in-out infinite;
}

@keyframes text {
  50% {
    color: black;
  }
}
</style>
</head>
<body>
<div class="center">
  <div class="ring"></div>
 <span>loading...</span>
</div>

</body>
</html>


