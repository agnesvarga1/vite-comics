<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <div id="wrapper">
    <div class="container">
      <div class="left-side">
        <div>
          <h3>Dc comics</h3>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <h3>Shop</h3>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div>
          <h3>Dc</h3>
          <ul>
            <li><a href="#">terms of use</a></li>
            <li><a href="#">privacy policy(new)</a></li>
            <li><a href="#">ad choices</a></li>
            <li><a href="#">advertising</a></li>
            <li><a href="#">jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">talent workshops</a></li>
            <li><a href="#">CPSC certificates</a></li>
            <li><a href="#">ratings</a></li>
            <li><a href="#">shop help</a></li>
            <li><a href="#">contact us</a></li>
          </ul>
        </div>
        <div>
          <h3>sites</h3>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD magazine</a></li>
            <li><a href="#">DC kids</a></li>
            <li><a href="#">DC universe</a></li>
            <li><a href="#">DC power visa</a></li>
          </ul>
        </div>
      </div>
      <div class="right-side">
        <figure>
          <img src="../../src/assets/img/dc-logo-bg.png" alt="" />
        </figure>
      </div>
    </div>
    <footer>
      <div class="footer-container">
        <button>sign-up now</button>
        <div>
          <h2>follow us</h2>
          <ul>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-facebook.png" alt="social"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-periscope.png" alt="social"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-pinterest.png" alt="social"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-twitter.png" alt="social"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-youtube.png" alt="social"
              /></a>
            </li>
          </ul>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
#wrapper {
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;

  color: #fff;
  .container {
    width: 75%;
    margin: 0 auto;
    padding-block: 4rem;
    display: flex;
    background: transparent;

    .left-side {
      width: 50%;
      display: flex;
      gap: 25px;
      line-height: 1.5;
      h3 {
        text-transform: uppercase;
        margin-block: 0.8rem;
      }
      li {
        a {
          font-size: 14px;
          color: #fff;
          font-weight: 100;
          opacity: 0.7;
          text-transform: capitalize;
        }
      }
    }
    .right-side {
      width: 50%;
      position: relative;
      figure {
        position: absolute;
        top: -120px;
      }
    }
  }
}
footer {
  background-color: #303030;
  position: absolute;
  width: 100%;
  .footer-container {
    width: 75%;
    margin: 0 auto;
    padding-block: 2rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
    button {
      padding: 1rem 2rem;
      background: transparent;
      border: 3px solid #0282f9;
      color: #fff;
      text-transform: uppercase;
      font-size: 18px;
      font-weight: bold;
    }
    div {
      display: flex;
      gap: 20px;
      align-items: center;
      h2 {
        color: #0282f9;
        text-transform: uppercase;
      }
      ul {
        display: flex;
        gap: 20px;
      }
    }
  }
}
</style>
