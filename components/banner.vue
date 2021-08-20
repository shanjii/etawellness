<template>
  <section id="banner">
    <span id="banner-filter">
      <div id="logo" @click="clickLogo()">
        <img src="/icons/logo.svg" alt="Logo of the ORG" />
      </div>
      <div class="contact">
        <div>
          <h3 class="number">732-285-5785</h3>
          <img
            class="phone"
            height="32"
            src="/icons/phone.svg"
            alt="Phone icon"
          />
        </div>
        <div>
          <h3 class="email">aredonet8@gmail.com</h3>
          <img class="mail" height="40" src="/icons/mail.svg" alt="Mail icon" />
        </div>
      </div>
    </span>
    <img
      v-if="easterEgg > 6"
      @click="easterEgg = 0"
      src="https://cdn.discordapp.com/emojis/684330616170348565.png"
      class="inigo"
      alt=""
    />
  </section>
</template>

<script>
export default {
  data: function () {
    return {
      easterEgg: 0,
      showInigo: false,
    };
  },
  methods: {
    clickLogo() {
      this.easterEgg++;
    },
  },
};
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
  background-image: linear-gradient(#000000b7, #00000000, #00000000);
  background-color: rgba(0, 0, 0, 0.39);
  width: 100%;
  height: 100%;
}
#logo {
  transition: linear 100ms;
  margin-top: 40px;
  margin-left: 40px;
}
.contact {
  position: absolute;
  top: 40px;
  right: 40px;
}
.contact > div {
  display: flex;
}
.phone {
  position: relative;
  top: -1px;
  margin-left: auto;
  margin-right: 10px;
}
.mail {
  position: relative;
  top: -3px;
  margin-left: auto;
  margin-right: 7px;
}

.number {
  color: white;
  margin-left: auto;
  margin-right: -59px;
  font-family: "Inter";
}

.email {
  color: white;
  margin-left: auto;
  margin-right: 10px;
  font-family: "Inter";
}

.inigo {
  cursor: pointer;
  position: absolute;
  transform: rotate(180deg);
  left: 30vw;
  animation: easteregg 2s;
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
  .contact {
    display: none;
  }
}

@keyframes easteregg {
  0% {
    transform: translateY(-200px) rotate(180deg);
  }
  100% {
    transform: translateY(0px) rotate(180deg);
  }
}
</style>