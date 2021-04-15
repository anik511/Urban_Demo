<template>
  <div class="card">
    <img :src="item.img" alt="Denim Jeans" style="width: 100%" />
    <h3>{{ item.name }}</h3>
    <p class="cat">{{ item.des }}</p>
    <p class="price">
      ${{ item.disprice }} <span>${{ item.price }}</span>
    </p>

    <a href="#">Add to Cart</a>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["item"],
};
</script>

<style scoped>
.card {
  max-width: 37rem;
  margin: auto;
  font-family: Playfair Display;
  text-align: left;
  color: #6e98a6;
}
.card h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 29px;
  margin: 1rem 0;
}
.cat {
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 25px;
  margin-bottom: 2rem;
}
.card img {
  width: 100%;
}
.products .col:nth-child(1) .card {
  margin-left: 0;
}

.price {
  font-family: Open Sans;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 25px;
  color: #b46254;
  margin-bottom: 2rem;
}
.price span {
  color: gray;
  margin-left: 2rem;
  text-decoration-line: line-through;
}
.card a {
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 25px;

  text-decoration-line: underline;

  color: #6e98a6;
}
</style>
