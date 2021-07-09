<template>
  <body>
    <div class="center">
      <img width="200px" class="inigo" src="images/inigo.png" />
    </div>
  </body>
</template>

<script>
export default {
  mounted() {
    var audio = new Audio('music.mp3');
    audio.play()
  }
};
</script>


<style scoped>
body {
  background-color: rgb(87, 87, 170);
  display: flex;
  width: 100vw;
  height: 100vh;
}
.center {
  display: flex;
  flex-direction: column;
  margin: auto;
}
.inigo {
  margin: auto;
  animation-name: inigo;
  border-radius: 100%;
  animation-duration: 3s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
.text {
  color: white;
  text-align: center;
  margin-top: 20px;
  font-size: 1.3rem;
}
@keyframes inigo {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
</style>
