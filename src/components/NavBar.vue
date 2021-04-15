<template>
  <nav>
    <div class="container">
      <a href="#">
        <img class="logo" src="../assets/Group 20.png" alt="logo" />
      </a>
      <ul class="left-nav">
        <li><a href="#">Home</a></li>
        <li><a href="#">Shop</a></li>
        <li><a href="#">Product</a></li>
        <li><a href="#">Page</a></li>
        <li><a href="#">Blog</a></li>
      </ul>
      <div class="icon-input">
        <input class="icon-input-text-field" type="text" />
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="#92B2BC"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="feather-find feather-search icon-input-icon"
        >
          <circle cx="11" cy="11" r="8"></circle>
          <line x1="21" y1="21" x2="16.65" y2="16.65"></line>
        </svg>
      </div>
      <ul class="right-nav">
        <li>
          <a class="cart" href="#"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              stroke="#6E98A6"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="feather feather-shopping-bag"
            >
              <path
                d="M6 2L3 6v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6l-3-4z"
              ></path>
              <line x1="3" y1="6" x2="21" y2="6"></line>
              <path d="M16 10a4 4 0 0 1-8 0"></path></svg
            ><span>Cart</span></a
          >
        </li>
        <li>
          <a class="cart" href="#"
            ><img class="profile" src="../assets/ami.jpg" alt="prfile" />
            <span>Alex Pitter</span></a
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  max-width: 144rem;
  padding: 0 13rem 0 13rem;
  box-sizing: border-box;
  height: 7rem;
}
.left-nav,
.icon-input,
.right-nav {
  display: flex;
  float: left;
  margin: 2.7rem auto;
}
.left-nav {
  font-family: Open Sans;
  font-size: 1.8rem;
  font-style: normal;
  font-weight: 400;
  line-height: 2.5rem;
  letter-spacing: 0em;
  margin-left: 6rem;
}
.left-nav a {
  color: #92b2bc;
}
.left-nav li {
  margin-right: 2.3rem;
}
ul li a:hover,
ul li a svg:hover {
  color: #dad398;
  stroke: #dad398;
}
/* search box */
.icon-input {
  position: absolute;
  width: 30rem;
  height: 2.4rem;
  left: 65rem;
}
.icon-input-text-field {
  width: 100%;
  border: 0px;
  border-bottom: 1px solid #92b2bc;
}
.icon-input-icon {
  position: absolute;
  top: 35%;
  right: 0rem;
  transform: translateY(-50%);
}
.icon-input-icon {
  color: #92b2bc;
}
.icon-input-text-field:focus {
  border: 0px !important;
  border-bottom: 2px solid #92b2bc !important;
  box-sizing: border-box;
}
.feather-find {
  width: 20px;
  height: 20px;
  stroke: currentColor;
  stroke-width: 1;
  stroke-linecap: round;
  stroke-linejoin: round;
  fill: none;
}
/* search box */
.logo {
  height: 4.86rem;
  width: auto;
  margin-top: 2rem;
  margin-bottom: 2rem;
  float: left;
}
.right-nav {
  display: flex;
  font-family: Open Sans;
  font-size: 1.8rem;
  font-style: normal;
  font-weight: 400;
  line-height: 2.5rem;
  letter-spacing: 0em;
  margin-left: 34rem;
}
.right-nav a {
  color: #92b2bc;
}
.right-nav a span {
  margin-left: 0.7rem;
}
.right-nav li {
  margin-right: 2rem;
}
.cart {
  display: flex;
}
.profile {
  width: 24px;
  height: 24px;
  top: 37px;
  border-radius: 50%;
  border: 1px solid #6e98a6;
  box-sizing: border-box;
}
</style>
