<template>
  <div class="collections">
    <h1>Featured in</h1>
    <div
      class="col span_1_of_6"
      v-for="(featured, index) in featureds"
      :key="index"
    >
      <a href="#">
        <img :class="['featured']" :src="featured.img" :alt="featured.name" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Partners",
  data() {
    return {
      featureds: [
        {
          nmae: "Featured-6",
          img: require("@/assets/img/XMLID 406.png"),
        },
        {
          nmae: "Featured-5",
          img: require("@/assets/img/XMLID 380.png"),
        },
        {
          nmae: "Featured-5",
          img: require("@/assets/img/XMLID 229.png"),
        },

        {
          nmae: "Featured-1",
          img: require("@/assets/img/XMLID 1.png"),
        },
        {
          nmae: "Featured-2",
          img: require("@/assets/img/Group 17.png"),
        },
        {
          nmae: "Featured-3",
          img: require("@/assets/img/XMLID 173.png"),
        },
      ],
    };
  },
};
</script>

<style scoped>
/* .collections {
  height: 35vh;
} */
.collections .col:nth-child(5) {
  margin-left: 0;
}
.featured {
  margin-top: -4.5rem;
  width: 67%;
}

.collections .col:nth-child(3) a img {
  margin-top: -7rem;
}
.collections h1 {
  margin-bottom: 7.4rem;
  color: #6e98a6;
  text-align: center;

  font-style: normal;
  font-weight: bold;
  font-size: 42px;
  line-height: 56px;
}
</style>
