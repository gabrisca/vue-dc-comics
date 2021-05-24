<template>
  <footer>
    <div class="footer-top container">
      <div class="footer-top-wrapper">
        <ul class="comics">
          <h3>DC COMICS</h3>
          <li>
            <a href="#">characters</a>
          </li>
          <li>
            <a href="#">comics</a>
          </li>
          <li>
            <a href="#">movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">games</a>
          </li>
          <li>
            <a href="#">videos</a>
          </li>
          <li>
            <a href="#">news</a>
          </li>
          <ul class="shop">
            <h3>SHOP</h3>
            <li>
              <a href="#">shop DC</a>
            </li>
            <li>
              <a href="#">shop DC collectibles</a>
            </li>
          </ul>
        </ul>

        <ul class="dc">
          <h3>DC</h3>
          <li>
            <a href="#">Terms Of Use</a>
          </li>
          <li>
            <a href="#">Privacy policy (new)</a>
          </li>
          <li>
            <a href="#">ad choices</a>
          </li>
          <li>
            <a href="#">advertising</a>
          </li>
          <li>
            <a href="#">jobs</a>
          </li>
          <li>
            <a href="#">subscriptions</a>
          </li>
          <li>
            <a href="#">talent workshops</a>
          </li>
          <li>
            <a href="#">CPSC certificates</a>
          </li>
          <li>
            <a href="#">ratings</a>
          </li>
          <li>
            <a href="#">shop help</a>
          </li>
          <li>
            <a href="#">contact us</a>
          </li>
        </ul>

        <ul class="sites">
          <h3>SITES</h3>
          <li>
            <a href="#">DC</a>
          </li>
          <li>
            <a href="#">MAD magazine</a>
          </li>
          <li>
            <a href="#">DC kids</a>
          </li>
          <li>
            <a href="#">DC universe</a>
          </li>
          <li>
            <a href="#">DC power visa</a>
          </li>
        </ul>
      </div>
    </div>

    <div class="footer-bottom container">
      <div class="btn">
        <a href="#">SIGN-UP NOW!</a>
      </div>
      <ul>
        <li>
          <a href="#">FOLLOW US</a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-facebook.png" alt="logo facebook" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-twitter.png" alt="logo twitter" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-youtube.png" alt="logo youtube" />
          </a>
        </li>
        <li>
          <a href="#">
            <img
              src="../assets/img/footer-pinterest.png"
              alt="logo pinterest"
            />
          </a>
        </li>
        <li>
          <a href="#">
            <img
              src="../assets/img/footer-periscope.png"
              alt="logo periscope"
            />
          </a>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
};
</script>

<style lang="scss" scoped>
// importo le variabili
@import "../assets/style/vars.scss";
footer {
  background-repeat: no-repeat;
  background-size: cover;
  background-image: url(../assets/img/footer-bg.jpg);
  .footer-top {
    .footer-top-wrapper {
      display: flex;
      justify-content: flex-start;
      background-image: url(../assets/img/dc-logo-bg.png);
      background-repeat: no-repeat;
      background-position-x: right;
      background-position-y: center;
      background-size: 32em;
      padding-top: 20px;
      padding-bottom: 40px;
      ul {
        flex-basis: 180px;
        margin-right: 20px;
        h3 {
          margin: 10px 0;
          color: white;
        }
        li {
          margin-bottom: 4px;
          a {
            color: #6c7b7c;
            text-decoration: none;
            text-transform: capitalize;
            &:hover {
              color: white;
            }
          }
        }
      }
    }
  }
  .footer-bottom {
    height: 100px;
    background-color: #303030;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .btn {
      border: 2px solid $brand-color;
      padding: 10px;
      cursor: pointer;
      &:hover {
        background-color: #8b7f7f17;
      }
      a {
        color: white;
      }
    }
    ul {
      display: flex;
      align-items: center;
      li {
        margin-left: 20px;
        &:first-child {
          font-size: 1.2em;
        }
        a {
          height: 100%;
          &:first-child {
            color: $brand-color;
          }
          img {
            &:hover {
              filter: brightness(1.8);
            }
          }
        }
      }
    }
  }
}
</style>
