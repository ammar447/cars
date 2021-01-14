<template>
  <div class="Header">
    <Nav></Nav>
    <Slider></Slider>
    <div class="new">
      <h1 style="color: #867979;">{{ findnew.title }}</h1>
      <div style=" font-size: 20px;">{{ findnew.text }}</div>
    </div>
    <Sale></Sale>
    <foot></foot>
  </div>
</template>

<script>
import Nav from "../components/Header/Navigation";
import Slider from "../components/Header/Sliderimag";
import Sale from "../components/Main/carsforsale";
import foot from "../components/ContactUs/ContactUs";
export default {
  name: "Home",
  components: {
    Nav,
    Slider,
    Sale,
    foot,
  },
  data() {
    return {
      findnew: {
        title: "Find you new or used car!",
        text:
          "Etiam quis viverra lorem, in semper lorem. Sed nisl arcu euismod sit amet nisi euismod sed cursus arcu elementum ipsum arcu vivamus quis venenatis orci lorem ipsum et magna feugiat veroeros aliquam. Lorem ipsum dolor sit amet nullam dolore.",
      },
    };
  },
};
</script>
<style scoped>
.new {
  margin-top: 25px;
  padding-left: 102px;
  padding-right: 10px;
  line-height: 1.9;
}
</style>
