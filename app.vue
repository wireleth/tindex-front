<template>
  <div>
    <div class="logo">

    <img src="~/public/tindex_logo.png" style="height: 30vh; width: auto;"  />
    <h1 class="tindx">Tindex</h1>
    <span class="looped-text 1"></span>
    </div>
  </div>
</template>

<style>
html, body {
  background-color: black;
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", 
  Helvetica, Arial, "Lucida Grande", sans-serif;
  color: white;
}
.tindex {
  font-size: 5rem;
}
.looped-text {
  padding-top: 0.5rem;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}
@keyframes change-text {
  0% {
    content: "Доверие";
  }
  33.3% {
    content: "Контроль";
}
  66.6% {
    content: "Результат";
  }
}
.looped-text::after {
  display: block;
  content: "Доверие";
/* animation-duration = number of keyframes * duration per keyframe */
  animation: change-text 5s infinite;
}
.logo {
height: 90vh;
display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
}
</style>
