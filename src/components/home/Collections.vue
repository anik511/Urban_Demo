<template>
  <div class="collections">
    <div class="col span_1_of_2 summer">
      <div>
        <a href="#">
          <img class="summer-crazy" src="../../assets/img/Group 3.png" alt=""
        /></a>
      </div>
      <div>
        <a href="#">
          <img
            class="summer-crazy"
            src="../../assets/img/Rectangle 7.png"
            alt=""
        /></a>
      </div>
    </div>
    <div class="col span_1_of_2 box">
      <a href="#">
        <img class="summer-crazy" src="../../assets/img/Group 4.png" alt=""
      /></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Collections",
};
</script>

<style scoped>
.collections {
  height: 94.34vh;
}
.summer div {
  height: 28rem;
  padding-bottom: 1.3rem;
  padding-top: 2rem;
}
.box {
  padding: 2rem;
}
.summer-crazy {
  width: 100%;
  height: 100%;
  border-radius: 1rem;
}
</style>
