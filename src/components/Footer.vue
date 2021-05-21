<template>
  <footer>
    <div class="footer-top container">
      <div class="footer-top-wrapper">
        <ul class="comics">
          <h3>DC COMICS</h3>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <ul class="shop">
            <h3>SHOP</h3>
            <li>
              <a href="#">link</a>
            </li>
            <li>
              <a href="#">link</a>
            </li>
          </ul>
        </ul>

        <ul class="dc">
          <h3>DC</h3>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
        </ul>

        <ul class="sites">
          <h3>SITES</h3>
          <li>
            <a href="#">dc</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
          </li>
          <li>
            <a href="#">link</a>
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
export default {};
</script>

<style lang="scss" scoped>
// importo le variabili
@import "../assets/style/vars.scss";
footer {
  background-color: honeydew;
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
        flex-basis: 150px;
        margin-right: 10px;
        h3 {
          margin: 10px 0;
          color: white;
        }
        li {
          a {
            color: #6c7b7c;
            text-decoration: none;
            &:hover {
              color: $brand-color;
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
    }
    ul {
      display: flex;
      align-items: center;
      li {
        margin-left: 20px;
        &:first-child {
          // line-height: 100px;
          font-size: 1.2em;
        }
        a {
          height: 100%;
          &:first-child {
            color: $brand-color;
          }
        }
      }
    }
  }
}
</style>
