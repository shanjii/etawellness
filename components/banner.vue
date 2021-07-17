<template>
  <section id="banner">
    <span id="banner-filter">
      <div id="logo">
        <img src="/icons/logo.svg" alt="" />
      </div>
    </span>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#banner {
  display: flex;
  height: 454px;
  width: 100vw;
  background-image: url("/images/banner.jpg");
  background-size: cover;
  background-position: center;
}
#banner-filter {
  display: flex;
  background-color: rgba(0, 0, 0, 0.39);
  width: 100%;
  height: 100%;
}
#logo {
    margin-top: 40px;
    margin-left: 40px;
}
</style>