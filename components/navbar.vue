<template>
  <section id="navbar">
    <ul class="button-region">
      <li>
        <p>MISSION</p>
      </li>
      <li>
        <p>GROUPS</p>
      </li>
      <li>
        <p>LOCATION</p>
      </li>
      <li>
        <p>DONATE</p>
      </li>
    </ul>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#navbar {
  position: absolute;
  top: 384px;
  z-index: 2;
  display: flex;
  height: 70px;
  width: 100vw;
  background-color: rgba(0, 0, 0, 0.562);
}
.button-region {
  display: flex;
  margin-left: auto;
  margin-right: auto;
}
li{
    display: flex;
    padding-left: 60px;
    padding-right: 60px;
    height: 100%;
}
p{
    color: white;
    align-self: center;
}
</style>