<template>
  <section id="navbar">
    <div class="button-region">
      <li>
        <p>MISSION</p>
        <img height="28px" class="icon" src="/icons/flag.svg" alt="" />
      </li>
      <li>
        <p>GROUPS</p>
        <img height="28px" class="icon" src="/icons/group.svg" alt="" />
      </li>
      <li>
        <p>LOCATION</p>
        <img height="28px" class="icon" src="/icons/location.svg" alt="" />
      </li>
      <li>
        <p>DONATE</p>
        <img height="30px" class="icon" src="/icons/donate.svg" alt="" />
      </li>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#navbar {
  user-select: none;
  transition: linear 100ms;
  margin-top: -70px;
  z-index: 2;
  display: flex;
  height: 70px;
  width: 100%;
  background-color: rgba(0, 0, 0, 0.562);
}
.button-region {
  display: flex;
  margin-left: auto;
  margin-right: auto;
  width: 80%;
  justify-content: space-around;
}
li {
  transition: ease-in 200ms;
  display: flex;
  height: 100%;
  cursor: pointer;
  padding-right: 60px;
  padding-left: 60px;
}
li:hover {
  background-color: rgba(150, 150, 150, 0.295);
}
p {
  color: white;
  font-family: "Inter";
  align-self: center;
}
img {
  align-self: center;
}
.icon {
  margin-left: 10px;
}
.navbar-scrolled {
  position: fixed;
  top: 70px;
}
@media (max-width: 1000px) {
  li {
    flex-direction: column;
  }
  .icon {
    margin-left: 0px;
    margin-top: auto;
    margin-bottom: auto;
  }
  p {
    display: none;
  }
  #navbar {
    margin-top: -70px;
  }
  .button-region {
    width: 100%;
  }
  li {
    padding-right: 20px;
    padding-left: 20px;
  }
 
}
</style>