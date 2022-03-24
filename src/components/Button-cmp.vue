<template>
  <div class="button">
    <h1>
      <button>{{ text }}</button>
    </h1>
  </div>
</template>
<script>
export default {
  name: 'Button',
  props: {
    text: {
      type: String,
    },
  },
};
</script>
<style scoped>
.button button {
  background: #333333;
  font-family: 'Space Mono';
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 21px;
  letter-spacing: -0.035em;
  text-transform: uppercase;
  color: #ffffff;
  padding: 22px 43px;
}
@media screen and (max-width: 1250px) {
  .button {
    display: flex;
    justify-content: flex-start;
    width: 70vw;
    height: 50%;
  }
}
</style>
