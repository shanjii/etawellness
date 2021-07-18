<template>
  <section>
    <Banner />
    <Navbar />
    <span></span>
  </section>
</template>

<script>
var scrolled, scrollSize, width;
export default {
  mounted() {
    this.updateWidth();
    window.onresize = () => {
      this.updateWidth();
    };
    window.onscroll = () => {
      scrolled = document.documentElement.scrollTop;
      if (scrolled >= scrollSize) {
        document.getElementById("navbar").classList.add("navbar-scrolled");
      } else {
        document.getElementById("navbar").classList.remove("navbar-scrolled");
      }
    };
  },
  methods: {
    updateWidth() {
      width = window.innerWidth;
      width > 1000 ? (scrollSize = 384) : (scrollSize = 184);
    },
  },
};
</script>


<style scoped>
span {
  display: flex;
  height: 2000px;
  background-color: rgb(226, 226, 226);
}
</style>
