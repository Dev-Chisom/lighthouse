<template>
  <div>
    <header class="hero hero__parallax">
      <Header />
      <!-- hero-section -->
      <div class="hero__left"></div>
      <div class="hero__content">
        <div class="hero__content-text">
          <h1 class="hero__content-heading">
            We Exist To <br />
            Honor God And <br />
            Make Disciples
          </h1>
          <div class="hero__content-buttons">
            <nuxt-link to="/events" class="hero__content-button">
              Upcomming Events
            </nuxt-link>
            <nuxt-link to="/about" class="hero__content-button">
              About Us
            </nuxt-link>
          </div>
        </div>
      </div>
      <!-- hero-socials -->
      <ul class="hero__socials">
        <li class="hero__socials-title">Follow</li>
        <li class="hero__social">
          <a href="">Facebook</a>
        </li>
        <li class="hero__social">
          <a href="">TouTube</a>
        </li>
        <li class="hero__social">
          <a href="">Instagram</a>
        </li>
      </ul>
    </header>
  </div>
</template>

<script>
import Header from "@/components/Navigation/Header";
export default {
  components: {
    Header
  }
};
</script>
<style lang="scss" scoped>
@keyframes fadeIn {
  0% {
    opacity: 0;
    visibility: hidden;
    -webkit-transform: translate3d(0, 100%, 0);
    transform: translate3d(0, 100%, 0);
  }
  100% {
    opacity: 1;
    visibility: visible;
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
}

.hero {
  width: 100%;
  height: 100vh;
  min-height: 82rem;
  overflow: hidden;
  background-color: transparent;
  position: relative;

  &__parallax {
    background-image: url("@/assets/images/hero-bg-3000.jpg");
    min-height: 700px;
    /* height: 700px; */
    object-fit: contain;
    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  &__parallax::before {
    display: block;
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #050505;
    opacity: 0.5;
  }
  &__left {
    height: 100%;
    width: 5rem;
    background-color: #000;
    opacity: 0.9;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
  }
  &__content {
    max-width: 1200px;
    height: 100%;
    /* padding-top: 20vh; */
    padding-bottom: 18vh;
    align-items: flex-end;
    position: relative;
    width: 89%;
    margin: 0 auto;
    display: flex;
    flex-flow: row wrap;
    animation-duration: 2s;
    -webkit-animation-duration: 2s;
    -webkit-animation-name: fadeIn;
    animation-name: fadeIn;
  }
  &__content-text {
    position: relative;
    display: flex;
    flex: 0 0 100%;
    max-width: 100%;
    padding: 0 20px;
  }
  &__content-heading {
    font-weight: 700;
    font-size: 3.5rem;
    line-height: 1.263;
    letter-spacing: 0;
    color: #ffffff;
    margin-top: 0;
    margin-left: 100px;
    margin-right: 200px;
    bottom: 3.2rem;
    /* padding-top: 3.2rem; */
    position: relative;
  }
  &__content-heading::before {
    display: block;
    content: "";
    height: 2px;
    width: 7rem;
    background-color: #7d1c24;
    position: absolute;
    top: -15px;
    left: 0.8rem;
  }
  &__content-buttons {
    position: absolute;
    right: 3rem;
    bottom: 3.2rem;
  }
  &__content-button {
    display: block;
    color: #fff;
    width: 30rem;
    margin-right: 0;
    background: transparent;
    border: 0.2rem solid #fff;
    font-family: "Montserrat", sans-serif;
    font-weight: 700;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 0.6rem;
    height: 6rem;
    line-height: 5.6rem;
    padding: 0 3.2rem;
    margin: 0 0.4rem 1.6rem 0;

    text-decoration: none;
    text-align: center;
    white-space: nowrap;
    cursor: pointer;
    transition: all 0.3s ease-in-out;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
}
</style>
