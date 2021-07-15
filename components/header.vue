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
        <a class="navbar-button" href="#"><b>Home</b></a>
        <a class="navbar-button" href="#"><b>Meanings</b></a>
        <a class="navbar-button" href="#"><b>About</b></a>
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
  border-radius: 100px;
}

#navbar > nav {
  display: flex;
  width: 100%;
  justify-content: space-around;
}

.navbar-button {
  background-color: rgb(92, 92, 92);
  width: 100%;
  text-align: center;
  padding: 13px;
}
.navbar-button:hover {
  background-color: rgb(167, 167, 167);
}
.navbar-button:first-child {
  border-top-left-radius: 100px;
  border-bottom-left-radius: 100px;
}
.navbar-button:last-child {
  border-top-right-radius: 100px;
  border-bottom-right-radius: 100px;
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
@media (max-width: 1000px) {
  .logo {
    margin-right: 0px;
  }
  #banner > div {
    display: flex;
    width: 100%;
    justify-content: space-between;
    padding-left: 10px;
    padding-right: 10px;
  }
  #navbar {
    width: 90%;
  }
}
</style>