<template>
  <main>
    <div class="container">
      <Card
        v-for="(element, index) in comics"
        :key="index"
        :thumb="element.thumb"
        :series="element.series"
      />
    </div>
  </main>
</template>

<script>
import Card from "./Card";

export default {
  name: "Main",
  components: {
    Card,
  },
  props: {
    comics: Array,
  },
};
</script>


<style scoped lang="scss">
@import "../style/colors";

main {
  background-color: black;
}

.container{
  display: flex;
  flex-wrap: wrap;
}
</style>