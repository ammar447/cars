<template>
  <div>
    <Nav></Nav>

    <div class="about">
      <h1>About Us</h1>
      <div class="inner">
        <img src="../assets/4.jpg" alt="" />
      </div>
      <div class="text">
        {{ text }}
      </div>
    </div>
    <foot></foot>
  </div>
</template>
<script>
import Nav from "../components/Header/Navigation";
import foot from "../components/footer/footer";
export default {
  components: {
    Nav,
    foot,
  },
  data() {
    return {
      text:
        "Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Curabitur sapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique.Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fersapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique lorem ipsum dolor.",
    };
  },
};
</script>
<style scoped>
.about {
  width: 100%;
  max-width: 72em;
  margin: 0 auto;
  padding: 0 2.5em;
  color: rgb(134, 121, 121);
  line-height: 2.5;
}
.about h1 {
  font-size: 2.75em;
  font-weight: 700;
  line-height: 1.3;
  margin: 100px 0 1px 0;
}
.about .inner img {
  display: block;
  width: 100%;
  height: 300px;
}
.about .text {
  line-height: 2.5;
  font-size: 24px;
}
</style>
