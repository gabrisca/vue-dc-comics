<template>
  <footer class="container">
    <div class="footer-top">
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

    <div class="footer-bottom">
      <div class="btn">
        <a href="#">SIGN-UP NOW!</a>
      </div>
      <ul>
        <li>
          <a href="#">FOLLOW US</a>
        </li>
        <li>
          <a href="#">FOLLOW US</a>
        </li>
        <li>
          <a href="#">FOLLOW US</a>
        </li>
        <li>
          <a href="#">FOLLOW US</a>
        </li>
        <li>
          <a href="#">FOLLOW US</a>
        </li>
        <li>
          <a href="#">FOLLOW US</a>
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
    display: flex;
    justify-content: flex-start;
    padding-top: 20px;
    padding-bottom: 40px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position-x: right;
    background-position-y: center;
    background-size: 32em;
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
  .footer-bottom {
    background-color: red;
  }
}
</style>
