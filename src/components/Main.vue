<template>
  <main>
    <div class="container">
      <Card
        v-for="(element, index) in comics"
        :key="index"
        :thumb="element.thumb"
        :series="element.series"
      />
      <ButtonLoad/>
    </div>
  </main>
</template>


<script>
  import Card from "./Card";
  import ButtonLoad from "./ButtonLoad";

  export default {
    name: "Main",
    components: {
      Card,
      ButtonLoad,
    },
    props: {
      comics: Array,
    },
  };
</script>


<style scoped lang="scss">
  @import "../style/colors";

  main {
    background-color: $bg-gray-main;
  }

  .container{
    display: flex;
    flex-wrap: wrap;
  }
</style>