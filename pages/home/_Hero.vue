<template>
  <div>
    <header class="hero hero__parallax">
      <Header />
      <div class="hero__left"></div>
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
.hero {
  width: 100%;
  height: 100vh;
  min-height: 82rem;
  overflow: hidden;
  background-color: transparent;
  position: relative;

  &__parallax {
    background-image: url("@/assets/images/herobg.jpg");
    /* min-height: 500px; */
    height: 2000px;
    object-fit: contain;
    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
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
}
</style>
