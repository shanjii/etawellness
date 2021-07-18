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
          alt="Flag icon"
        />
        <h3>Our Mission</h3>
      </div>
      <p>
        Welcome to ETA Wellness Anxiety Support Group.
        <br /><br />
        Our mission is to provide peer support for individuals suffering from
        <b>anxiety</b> or <b>anxiety disorders.</b>

        We operate in accordance with the belief that peer support is an
        effective way to combat hopelessness, gain new perspectives, and share
        effective coping strategies to manage and maintain wellness.
      </p>
    </section>
    <div id="groups" class="box-div">
      <section class="left-box">
        <div class="title-left">
          <img
            class="icon-large"
            height="110px"
            src="/icons/group.svg"
            alt="Flag icon"
            srcset=""
          />
          <h3>Groups</h3>
        </div>
        <p class="offset">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
          tristique leo et sollicitudin pharetra. Duis pretium enim ac pulvinar
          eleifend. Sed lobortis quam quis enim rutrum viverra. Proin maximus
          interdum volutpat. Nam lorem lectus, egestas ac lorem vitae, varius
        </p>
      </section>
      <section class="image-box">
        <img src="/images/group.jpg" alt="People holding hands" srcset="" />
      </section>
    </div>
    <section id="guide" class="middle-box">
      <div class="title-middle">
        <img
          class="icon-large"
          height="190px"
          src="/icons/manual.svg"
          alt="Guide icon"
          srcset=""
        />
        <h3>Newcomer’s Guide</h3>
      </div>
      <p>Free and Informative!</p>
      <Button />
    </section>
    <div id="location" class="box-div">
      <section class="image-box">
        <img src="/images/church.jpg" alt="Image of a church" />
      </section>
      <section class="right-box">
        <div class="title-right">
          <h3>Location</h3>
          <img
            class="icon-large"
            height="110px"
            src="/icons/location.svg"
            alt="Location icon"
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
    <section class="middle-box">
      <h3>Find us on the map!</h3>
      <div class="map-div">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2728.5690557318303!2d9.515269215840465!3d46.85217274777898!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4784c70c74cbe553%3A0x7fee9a2fe1ba1049!2sHemaris%20AG!5e0!3m2!1sen!2sbr!4v1626597293940!5m2!1sen!2sbr"
          width="90%"
          height="550"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
        ></iframe>
      </div>
    </section>
  </section>
</template>

<script>
var scrolled, scrollSize, width;
export default {
  mounted() {
    var navbar = document.getElementById("navbar");
    this.updateWidth();
    window.onresize = () => {
      this.updateWidth();
    };
    window.onscroll = () => {
      scrolled = document.documentElement.scrollTop;
      if (scrolled >= scrollSize) {
        navbar.classList.add("navbar-scrolled");
      } else {
        navbar.classList.remove("navbar-scrolled");
      }
    };
  },
  methods: {
    updateWidth() {
      width = window.innerWidth;
      width > 1000 ? (scrollSize = window.innerHeight - 70) : (scrollSize = 184);
    },
  },
};
</script>


<style scoped>
@import "~/assets/main.css";
</style>
