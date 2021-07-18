<template>
  <section>
    <Banner />
    <Navbar />
    <section id="mission" class="middle-box">
      <div class="title-middle">
        <img
          class="icon-large"
          height="110px"
          src="/icons/flag.svg"
          alt=""
          srcset=""
        />
        <h3>Our Mission</h3>
      </div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam tristique
        leo et sollicitudin pharetra. Duis pretium enim ac pulvinar eleifend.
        Sed lobortis quam quis enim rutrum viverra. Proin maximus interdum
        volutpat. Nam lorem lectus, egestas ac lorem vitae, varius tempor
        tellus. Ut vehicula ante et velit aliquam, eget posuere orci ultricies.
        Duis convallis malesuada tortor, quis scelerisque ipsum malesuada sed.
        Cras vitae leo tellus. Aenean dictum nibh vitae ex volutpat euismod.
        Etiam quis purus purus. Donec vel dolor leo. Suspendisse in ante quam.
        Proin accumsan imperdiet risus, eu volutpat ipsum blandit sed. Mauris
        tincidunt accumsan facilisis. Integer fringilla ultrices tellus.
      </p>
    </section>
    <div id="groups" class="box-div">
      <section class="left-box">
        <div class="title-left">
          <img
            class="icon-large"
            height="110px"
            src="/icons/group.svg"
            alt=""
            srcset=""
          />
          <h3>Groups</h3>
        </div>
        <p class="offset">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
          tristique leo et sollicitudin pharetra. Duis pretium enim ac pulvinar
          eleifend. Sed lobortis quam quis enim rutrum viverra. Proin maximus
          interdum volutpat. Nam lorem lectus, egestas ac lorem vitae, varius
          tempor tellus. Ut vehicula ante et velit aliquam, eget posuere orci
          ultricies. Duis convallis malesuada tortor, quis scelerisque ipsum
          malesuada sed. Cras vitae leo tellus. Aenean dictum nibh vitae ex
          volutpat euismod. Etiam quis purus purus. Donec vel dolor leo.
          Suspendisse in ante quam. Proin accumsan imperdiet risus, eu volutpat
          ipsum blandit sed. Mauris tincidunt accumsan facilisis. Integer
          fringilla ultrices tellus.
        </p>
      </section>
      <section class="image-box">
        <img src="/images/group.jpg" alt="" srcset="" />
      </section>
    </div>
    <div id="location" class="box-div">
      <section class="image-box">
        <img src="/images/church.jpg" alt="" srcset="" />
      </section>
      <section class="right-box">
        <div class="title-right">
          <h3>Location</h3>
          <img
            class="icon-large"
            height="110px"
            src="/icons/location.svg"
            alt=""
            srcset=""
          />
        </div>
        <p class="offset">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
          tristique leo et sollicitudin pharetra. Duis pretium enim ac pulvinar
          eleifend. Sed lobortis quam quis enim rutrum viverra. Proin maximus
          interdum volutpat. Nam lorem lectus, egestas ac lorem vitae, varius
          tempor tellus. Ut vehicula ante et velit aliquam, eget posuere orci
          ultricies. Duis convallis malesuada tortor, quis scelerisque ipsum
          malesuada sed. Cras vitae leo tellus. Aenean dictum nibh vitae ex
          volutpat euismod. Etiam quis purus purus. Donec vel dolor leo.
          Suspendisse in ante quam. Proin accumsan imperdiet risus, eu volutpat
          ipsum blandit sed. Mauris tincidunt accumsan facilisis. Integer
          fringilla ultrices tellus.
        </p>
      </section>
    </div>
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
@import "~/assets/main.css";
</style>
