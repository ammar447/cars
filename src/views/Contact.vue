<template>
  <div>
    <Nav></Nav>
    <googlemap />
    <contact />
  </div>
</template>

<script>
import Nav from "../components/Header/Navigation";
import googlemap from "../components/googlemap";
import contact from "../components/ContactUs/ContactUs";
export default {
  name: "Contact",
  components: {
    Nav,
    googlemap,
    contact,
  },
};
</script>

<style scoped></style>
