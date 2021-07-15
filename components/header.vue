<template>
  <div id="header">
    <section id="banner">
      <div>
        <h3 class="logo">ETAWellness Logo</h3>
        <p class="slogan">Slogan</p>
      </div>
    </section>
    <section id="navbar">
      <nav>
        <a href="#"><b>Home</b></a>
        <a href="#"><b>Meanings</b></a>
        <a href="#"><b>About</b></a>
      </nav>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#header {
  display: flex;
  z-index: 999;
  width: 100%;
  margin-left: auto;
  margin-right: auto;
  flex-direction: column;
  align-items: center;
}
h3 {
  font-size: 25px;
}
#banner {
  display: flex;
  background-color: rgb(255, 255, 255);
  width: 100%;
}
#banner > div {
  display: flex;
  padding: 40px;
}
#navbar {
  display: flex;
  width: 60%;
  z-index: 999;
  position: relative;
  top: -15px;
  background-color: rgb(100, 100, 100);
  border-radius: 100px;
}

#navbar > nav {
  display: flex;
  width: 100%;
  padding: 13px;
  justify-content: space-around;
}
.logo {
  margin-top: auto;
  margin-right: 100px;
  margin-bottom: auto;
}
.slogan {
  margin-top: auto;
  margin-bottom: auto;
}
a {
  color: white;
  text-decoration: none;
}
</style>