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
  transition: linear 100ms;
  display: flex;
  height: 454px;
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
  transition: linear 100ms;
  margin-top: 40px;
  margin-left: 40px;
}

@media (max-width: 1000px) {
  #banner {
    height: 254px;
    background-image: url("/images/banner.jpg");
    background-size: cover;
    background-position: center;
  }
  #logo {
    margin-top: 20px;
    margin-left: 10px;
  }
  img {
    width: 150px;
  }
}
</style>