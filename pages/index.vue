<template>
  <body>
    <div class="center">
      <img class="inigo" src="images/inigo.png" />
      <p class="text">If you can read me that means it's working.</p>
    </div>
  </body>
</template>

<script>
export default {};
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
