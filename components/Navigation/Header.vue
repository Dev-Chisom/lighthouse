<template>
  <nav class="header">
    <div class="header__logo">
      <nuxt-link to="/home" class="logo">
        <!-- <img src="~/assets/images/light.png" alt=""
      /> -->LightHouse
      </nuxt-link>
    </div>
    <nav class="header__nav-wrap">
      <ul class="header__nav">
        <li class="header__links">
          <nuxt-link class="header__link" to="/home">Home</nuxt-link>
        </li>
        <li class="header__links">
          <nuxt-link class="header__link" to="/about">About</nuxt-link>
        </li>
        <li class="header__links">
          <nuxt-link class="header__link" to="/happenings">Events</nuxt-link>
        </li>
        <li class="header__links">
          <nuxt-link class="header__link" to="/contact">Contacts</nuxt-link>
        </li>
      </ul>
    </nav>
  </nav>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss" scoped>
img {
  /* width: 128px;
  height: 49px; */
  object-fit: cover;
}
.logo {
  text-transform: uppercase;
  letter-spacing: 0.1rem;
  color: rgba(255, 255, 255, 0.8);
}
.header {
  z-index: 100;
  height: 7.2rem;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: transparent;

  &__logo {
    z-index: 102;
    transition: all 0.3s;
    transform: translate3d(0, -50%, 0);
    margin: 0 0.8rem;
    margin-left: 6rem;
    font-size: 1.5rem;
    width: 50px;
    height: 20px;
  }
  /* &__logo::before {
    content: "";
    display: block;
    background-color: rgba(255, 255, 255, 0.5);
    height: 1px;
    width: 9rem;
    position: absolute;
    top: 50%;
    left: -11rem;
  } */
  &__nav-wrap {
    z-index: 101;
  }
  &__nav {
    display: flex;
    align-items: center;
    justify-content: space-around;
    list-style: none;
    font-family: "Montserrat", sans-serif;
    font-size: 0.7rem;
    line-height: 4.8rem;
    text-transform: uppercase;
    letter-spacing: 0.35rem;
  }
  &__links {
    margin: 0 0.8rem;
  }
  &__link {
    color: rgba(255, 255, 255, 0.8);
    /* color: #000; */
    transition: all 0.3s ease-in-out;
  }
}
</style>
