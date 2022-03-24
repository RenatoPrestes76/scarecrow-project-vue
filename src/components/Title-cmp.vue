<template>
  <div class="title">
    <h1 v-if="level === 1">
      <slot></slot>
    </h1>
    <h2 v-else-if="level === 2">
      <slot></slot>
    </h2>
    <h3 v-else-if="level === 3">
      <slot></slot>
    </h3>
    <h4 v-else-if="level === 4">
      <slot></slot>
    </h4>
    <h5 v-else-if="level === 5">
      <slot></slot>
    </h5>
    <h6 v-else-if="level === 6">
      <slot></slot>
    </h6>
  </div>
</template>
<script>
export default {
  name: 'Title',
  props: {
    level: {
      type: Number,
      Required: true,
    },
  },
};
</script>
<style scoped>
.title {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
}
h1 {
  font-family: 'Space Mono';
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 80px;
  letter-spacing: -0.035em;
  color: #333333;
  width: 40vw;
  height: 20vh;
  margin: 0;
}
@media screen and (max-width: 1250px) {
  .title {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: flex-start;
    width: 100%;
  }
  h1 {
    font-family: 'Space Mono';
    font-style: normal;
    font-weight: 900;
    font-size: 35px;
    line-height: 40px;
    letter-spacing: -0.035em;
    color: #333333;
    width: 80vw;
    height: 10vh;
    margin: 0%;
  }
}
</style>
