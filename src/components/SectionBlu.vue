<template>
  <section>
    <div class="container">
      <div class="col">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <span>DIGITAL COMICS</span>
      </div>
      <div class="col">
        <img src="../assets/buy-comics-merchandise.png" alt="" />
        <span>DC MECHANDISE</span>
      </div>
      <div class="col">
        <img src="../assets/buy-comics-subscriptions.png" alt="" />
        <span>SUBSCRIPTION</span>
      </div>
      <div class="col">
        <img src="../assets/buy-comics-shop-locator.png" alt="" />
        <span>COMIC SHOP LOCATOR</span>
      </div>
      <div class="col">
        <img src="../assets/buy-dc-power-visa.svg" alt="" />
        <span>CD POWER VISA</span>
      </div>
    </div>
  </section>
</template>


<script>
  export default {
    name: "SectionBlu",
  };
</script>


<style scoped lang="scss">
  @import "../style/colors";

  section {
    background-color: $dc-blue-color;
    padding: 30px 0;
  }
  .container {
    display: flex;

    .col {
      width: calc(100% / 5);

      img {
        height: 50px;
        vertical-align: middle;
        padding-right: 20px;
      }

      span {
        color: $text-white;
        font-family: "Roboto Condensed", sans-serif;
      }
    }
  }
</style>