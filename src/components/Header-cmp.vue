<template>
  <div class="header">
    <h1>{{ text }}</h1>
  </div>
</template>
<script>
export default {
  name: 'Header',
  props: {
    text: {
      type: String,
    },
  },
};
</script>
<style scoped>
.header {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: flex-start;
  width: 50%;
  margin: 0;
}
h1 {
  font-family: 'Inconsolata';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 25px;
  letter-spacing: -0.08em;
  text-transform: uppercase;
  color: #333333;
  margin: 2% 0 0 3%;
}
</style>
