<template>
  <main>
    <div class="container">
        <button class="btn"> LOAD MORE</button>
    </div>
  </main>
</template>


<script>

  export default {
    name: "Button",

  };

</script>


<style scoped lang="scss">

  @import "../style/colors";

  .container{
    text-align: center;
    
    .btn{
      width: 150px;
      line-height: 34px;
      margin: 20px 0;
      background-color: $dc-blue-color;
      border: 0;
      color: $text-white;
      cursor: pointer;
      font-weight: bold;
    }
  }
</style>