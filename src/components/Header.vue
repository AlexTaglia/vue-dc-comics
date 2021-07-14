<template>
  <header class="container">
    <nav>
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="Logo DC" />
      </div>

      <div class="menu">
        <ul>
          <li v-for="element in navList" :key="element.id">
            <a :href="element.link">{{ element.name }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
  import navJson from "../jsons/nav-list";

  export default {
    name: "Header",

    data: function () {
      return {
        navList: navJson,
      };
    },
  };
</script>


<style scoped lang="scss">
  @import "../style/colors";

  header {
    height: 80px;
    padding: 10px 0;

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;

      img {
        height: 60px;
      }

      ul {
        display: flex;

        li {
          a {
            color: black;
            font-family: "Roboto Condensed", sans-serif;
            font-weight: bold;
            margin-left: 24px;
            padding-bottom: 23px;
            text-transform: uppercase;

            &:hover {
              color: $dc-blue-color;
              border-bottom: 5px solid $dc-blue-color;
            }
          }
        }
      }
    }
  }
</style>
