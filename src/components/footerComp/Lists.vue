<template>
  <ul>
    <li v-for="(list, index) in lists" :key="index">
      <a :href="list.url">{{ list.title }}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "Lists",
  props: ["lists"],
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap");
ul li {
  font-family: "Open Sans", sans-serif;
  font-size: 1.8rem;
  line-height: 3.7rem;
  font-weight: 300;
}
a {
  color: #fff;
}
</style>
