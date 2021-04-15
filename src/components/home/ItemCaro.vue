<template>
  <div class="products">
    <h1>Meet our best selling products</h1>
    <p>
      “Best premium laxarious Brand authentic product always available for you”
    </p>
    <div v-for="(product, index) in products" :key="index" class="row">
      <div v-for="pro in product" :key="pro.id" class="col span_1_of_3">
        <Card :item="pro" />
      </div>
      <div class="crcl">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="feather feather-arrow-right"
        >
          <line x1="5" y1="12" x2="19" y2="12"></line>
          <polyline points="12 5 19 12 12 19"></polyline>
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "../Ui/Card.vue";
export default {
  components: {
    Card,
  },
  data() {
    return {
      products: [
        [
          {
            id: 1,
            img: require("@/assets/img/Rectangle 13.png"),
            name: "De Rose Gold Perfume",
            des: "Floral Green fragrance for women",
            disprice: 55.0,
            price: 75.0,
          },
          {
            id: 2,
            img: require("@/assets/img/Rectangle 14.png"),
            name: "La Classic Car perfume",
            des: "Floral fragrance for Car",
            disprice: 55.0,
            price: 75.0,
          },
          {
            id: 3,
            img: require("@/assets/img/Rectangle 15.png"),
            name: "De Casta Blue berry Centario",
            des: "Floral sharp berry  for women",
            disprice: 55.0,
            price: 75.0,
          },
        ],
        [
          {
            id: 1,
            img: require("@/assets/img/Rectangle 13-1.png"),
            name: "XOFOSR Bag",
            des: "Floral Green fragrance for women",
            disprice: 55.0,
            price: 75.0,
          },
          {
            id: 2,
            img: require("@/assets/img/Rectangle 14-1.png"),
            name: "MAC Jacobs collections",
            des: "Floral fragrance for Car",
            disprice: 55.0,
            price: 75.0,
          },
          {
            id: 3,
            img: require("@/assets/img/Rectangle 15-1.png"),
            name: "De Casta Styles Bag",
            des: "Floral sharp berry  for women",
            disprice: 55.0,
            price: 75.0,
          },
        ],
      ],
    };
  },
};
// JavaScript Document
</script>

<style scoped>
.products {
  box-sizing: border-box;
  margin-bottom: 8rem;
}
.products h1,
.products p {
  text-align: center;
}
.products h1 {
  font-family: Playfair Display;
  font-size: 42px;
  font-style: normal;
  font-weight: 700;
  line-height: 56px;
  letter-spacing: 0em;
  color: #6e98a6;
}
.products p {
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 27px;
  color: #dad398;
  margin-bottom: 3.5rem;
}
.crcl {
  height: 5rem;
  width: 5rem;
  border-radius: 50%;
  float: right;
  margin-right: 2.5rem;
  text-align: center;
  padding-top: 1.4rem;
  background: #6e98a6;
  color: white;
  margin: 175px 0px 0px 1095px;
  position: absolute;
}
.feather {
  width: 20px;
  height: 20px;
  stroke: currentColor;
  stroke-width: 2;
  stroke-linecap: round;
  stroke-linejoin: round;
  fill: none;
}
</style>
