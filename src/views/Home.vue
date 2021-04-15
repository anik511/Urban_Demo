<template>
  <div class="main-container">
    <section class="hero">
      <div class="row">
        <div class="col span_2_of_2">
          <div class="hero-view">
            <img src="../assets/img/Rectangle 3.png" alt="" />
          </div>
          <div class="hero-contant">
            <h1>New Fasion Trends for Summer</h1>
            <p>
              There are many variations of passages of Lorem Ipsum available,
              but the majority have suffered alteration in some form, by
              injected humour, or randomised words.
            </p>
            <a href="#" class="btn btn-hero">Shop now</a>
          </div>
        </div>
      </div>
    </section>
    <div class="sub-con">
      <Collections /><item-caro></item-caro> <Products /><Partners />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Collections from "@/components/home/Collections.vue";
import Products from "@/components/home/Products.vue";
import Partners from "@/components/home/Partners.vue";
import ItemCaro from "../components/home/ItemCaro.vue";

export default {
  name: "Home",
  components: {
    Collections,
    Products,
    Partners,
    ItemCaro,
  },
};
</script>
<style scoped>
.sub-con {
  padding: 0 6rem;
  box-sizing: border-box;
  margin: 0 auto;
}
.hero {
  border: 1px solid white;
}
.hero-view {
  float: left;
}
.hero-view img {
  position: absolute;
  max-width: 72.5rem;
}
.hero-contant {
  text-align: left;
  width: 56.3rem;
  float: right;
  background: linear-gradient(#6e98a6, #6e98a6),
    url("../assets/img/Group-2.png");
  padding: 5.5rem 7rem 10.6rem 7rem;
  color: #fff;
  border-radius: 0 1rem 1rem 0;
}
.hero-contant h1 {
  font-family: Playfair Display;
  font-style: normal;
  font-weight: 700;
  line-height: 56px;
  letter-spacing: 0em;
}
.hero-contant p {
  font-family: Open Sans;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  text-align: justify;
}
.btn {
  color: #fff;
  padding: 2rem 6rem;
  display: inline-block;
  border-radius: 0.3rem;
  margin-top: 3rem;
}
.btn-hero:link,
.btn-hero:visited {
  background-color: #dad398;
  font-family: Open Sans;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  border-radius: 0.5rem;
}
.col {
  margin-top: -20px !important;
  margin-bottom: 0 !important;
}
</style>
