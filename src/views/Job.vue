<template>
  <div>
    <Nav></Nav>
    <div class="Job">
      <div class="inner">
        <img src="../assets/4.jpg" alt="" />
      </div>
      <h1>Just send me your CV and wait:</h1>
      <v-file-input
        show-size
        counter
        multiple
        label=" Send Here "
      ></v-file-input>
    </div>

    <foot />
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
};
</script>
<style scoped>
.Job {
  width: 100%;
  max-width: 72em;
  margin: 0 auto;
  padding: 0 2.5em;
  color: rgb(134, 121, 121);
  line-height: 2.5;
}
h1 {
  margin-top: 100px;
}
.Job .inner img {
  margin-top: 125px;

  display: block;
  width: 100%;
  height: 300px;
}
</style>
