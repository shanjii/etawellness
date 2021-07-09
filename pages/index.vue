<template>
  <body>
    <div class="center">
      <img @click="click" width="200px" id="inigo" src="images/inigo.png" />
    </div>
  </body>
</template>

<script>
var audio = new Audio("music.mp3");
export default {
  methods: {
    click() {
      audio.play();
      document.getElementById('inigo').classList.add('animate')
    },
  },
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
#inigo {
  margin: auto;
  border-radius: 100%;
}

.animate{
  animation-name: inigo;
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
