<template>
  <v-carousel :show-arrows="false">
    <v-carousel-item
      id="small"
      v-for="(item, i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: require("../../assets/1.jpg"),
        },
        {
          src: require("../../assets/2.jpg"),
        },
        {
          src: require("../../assets/3.jpg"),
        },
      ],
    };
  },
};
</script>
<style scoped>
@media screen and (max-width: 736px) {
  #small {
    width: auto;
  }
}
</style>
