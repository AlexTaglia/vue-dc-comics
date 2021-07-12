<template>
  <footer>
    <section class="section-link">
      <div class="container">
        <div class="left-side">
          <div class="col">
            <ul>
              <li class="bold">DC COMICS</li>
              <li><a href="">Characters</a></li>
              <li><a href="">Characters</a></li>
              <li><a href="">Characters</a></li>
              <li><a href="">Characters</a></li>
              <li><a href="">Characters</a></li>
              <li><a href="">Characters</a></li>
              <li><a href="">Characters</a></li>
            </ul>
            <ul>
              <li class="bold">SHOP</li>
              <li><a href="">Shop DC</a></li>
              <li><a href="">Shop DC Collectibles</a></li>
            </ul>
          </div>

          <div class="col">
            <ul>
              <li class="bold">DC</li>
              <li><a href="">Terms of Use</a></li>
              <li><a href="">Privacy policy (New)</a></li>
              <li><a href="">Ad choise</a></li>
              <li><a href="">Advertising</a></li>
              <li><a href="">Jobs</a></li>
              <li><a href="">Subscrition</a></li>
              <li><a href="">Talent Workshops</a></li>
              <li><a href="">CPSC Certificates</a></li>
              <li><a href="">Ratings</a></li>
              <li><a href="">Shop Help</a></li>
              <li><a href="">Contact Us</a></li>
            </ul>
          </div>

          <div class="col">
            <ul>
              <li class="bold">SITES</li>
              <li><a href="">DC</a></li>
              <li><a href="">MAD Magazine</a></li>
              <li><a href="">DC Kids</a></li>
              <li><a href="">DC Universe</a></li>
              <li><a href="">DC Power Visa</a></li>
            </ul>
          </div>
        </div>

        <div class="right-side">
          <img src="../assets/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </section>

    <section class="social"></section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>


<style scoped lang="scss">
.section-link {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  height: 400px;
  position: relative;

  .container {
    display: flex;
    justify-content: space-between;
  }

  .left-side {
    display: flex;

    li {
      color: white;
      padding: 5px 24px 0 0;

      &:first-child{
        font-weight: bold;
        padding-bottom: 6px;
      }
    }

    a {
      color: gray;
    }
  }

  .right-side {
    img {
      height: 300px;
      position: absolute;
      top: 50%;
      transform: translate(-100%, -50%);
    }
  }
}
</style>
