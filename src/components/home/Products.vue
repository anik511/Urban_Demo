<template>
  <div class="collections">
    <div class="title">
      <p>Clients Say about us</p>
      <h1>Testimonial</h1>
    </div>
    <div
      v-for="(review, index) in reviews"
      :key="index"
      class="col span_1_of_2"
    >
      <div class="card">
        <div class="image">
          <img :src="review.img" width="100%" />
        </div>

        <div class="text">
          <div class="fab">&#8220;</div>

          <h2>{{ review.title }}</h2>
          <p class="loc">{{ review.sp }}</p>
          <p class="review">
            {{ review.des }}
          </p>
        </div>
      </div>
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
</template>

<script>
export default {
  data() {
    return {
      reviews: [
        {
          id: 1,
          img: require("@/assets/img/Rectangle 16.png"),
          title: "Natasha Malina",
          sp: "Beauty Model in USA",
          des: `Every spring I start going through dress withdrawals and go crazy
            over all the pretty spring dresses that come out haha. It’s like
            famine and then feast and dresses`,
        },
        {
          id: 2,
          img: require("@/assets/img/Rectangle 19.png"),
          title: "Team Xodias",
          sp: "Fashion House",
          des: `Every spring I start going through dress withdrawals and go crazy
            over all the pretty spring dresses that come out haha. It’s like
            famine and then feast and dresses`,
        },
      ],
    };
  },
};
</script>

<style scoped>
.collections {
  height: 102.34vh;
  box-sizing: border-box;
  /* border: 1px solid red; */
}
.collections .col:nth-child(3) .card {
  margin: -71px 0px 0px 18px;
  padding: 0 0 0 1rem;
}
.collections .col:nth-child(2) .card {
  padding: 0 1rem 0 0;
}
.col {
  margin: 0;
}

.title p {
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;

  color: #dad398;
}
.title h1 {
  font-family: Playfair Display;
  font-style: normal;
  font-weight: bold;
  font-size: 42px;
  color: #6e98a6;
  margin-top: 2rem;
  margin-bottom: 0px;
}
.card {
  display: inline-block;
  margin: 20px 0;
  position: relative;
  margin-bottom: 50px;
  transition: all 0.2s ease-in-out;
}

.image {
  height: 25rem;
  opacity: 0.7;
  overflow: hidden;
  border-radius: 0.6rem;
  transition: all 0.2s ease-in-out;
}

.image:hover,
.card:hover .image {
  height: 25rem;
  opacity: 1;
}

.text {
  background: #fff;
  padding: 2rem;
  min-height: 20rem;
  font-family: Playfair Display;
  font-style: normal;
  padding-left: 0;
}
.text p {
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 25px;
  margin-top: 1rem;
}
.text .loc {
  color: #6e98a6;
}
.text .review {
  color: #767676;
}
.text h2 {
  font-weight: bold;
  font-size: 22px;
  line-height: 29px;
  color: #6e98a6;
}

.fab {
  width: 6rem;
  height: 5rem;
  position: absolute;
  margin-top: -5rem;
  right: 2rem;
  color: #fff;
  border-radius: 0.5rem;
  font-size: 6rem;
  font-weight: 800;
  text-align: center;
  background: #dad398;
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
  /* margin: 0px auto; */
  color: white;
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
