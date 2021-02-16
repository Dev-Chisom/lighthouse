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
          <a href="">YouTube</a>
        </li>
        <li class="hero__social">
          <a href="">Instagram</a>
        </li>
      </ul>
    </header>
    <!-- About Section -->
    <section class="about">
      <div class=" row about__content">
        <div class="column large-half">
          <h3 class="subhead">Welcome to Light House Africa</h3>
          <p class="lead">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. labore et dolore magna aliqua. Ut
            enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi
            ut aliquip ex ea commodo consequat.
          </p>
          <nuxt-link to="/about" class="btn btn--primary about__btn"
            >More About TLHA</nuxt-link
          >
        </div>
        <div class="column large-half meduim-full">
          <ul class="about__program">
            <li>
              <h4>Main Church Service</h4>
              <p>
                Sunday - 9:00 AM | 12:00 AM <br />
                Ndokwa Arena Event Center, 148 Itire Bus Stop, Ojo Road.
                Ajegunle Apapa, Lagos State
              </p>
            </li>
            <li>
              <h4>Kids Church Service</h4>
              <p>
                Sunday - 9:00 AM | 12:00 AM <br />
                Ndokwa Arena Event Center, 148 Itire Bus Stop, Ojo Road.
                Ajegunle Apapa, Lagos State
              </p>
            </li>
            <li>
              <h4>Prayer Meeting</h4>
              <p>
                Wednesday - 6:00 PM <br />
                Ndokwa Arena Event Center, 148 Itire Bus Stop, Ojo Road.
                Ajegunle Apapa, Lagos State
              </p>
            </li>
          </ul>
        </div>
      </div>
    </section>
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
.about {
  padding-top: 12rem;
  padding-bottom: 9rem;
  background-color: #3b0d11;
  color: rgba(255, 255, 255, 0.8);

  &__center {
    align-items: center;
  }
  &__center:first-child {
    padding-right: 2.4vw;
  }
  &__content .lead {
    margin-bottom: 3rem;
    color: #fff;
  }
  &__btn {
    display: block;
    width: 100%;
    margin-right: 0;
    background-color: #21070a;
    border-color: #21070a;
  }
  &__program {
    list-style: none;
    margin: 0;
    border-top: 1px solid rgba(255, 255, 255, 0.8);
  }
  &__program li {
    border-bottom: 1px solid rgba(255, 255, 255, 0.05);
    padding-top: 3.2rem;
    padding-left: 0;
  }
  &__program h4 {
    font-size: 1.5rem;
    line-height: 1.333;
    margin-top: 0.5rem;
    text-transform: uppercase;
    letter-spacing: 0.4rem;
    color: #ffffff;
  }
  &__program p {
    font-size: 1rem;
    line-height: 1.333;
    margin-top: 0.5rem;
  }
}
</style>
