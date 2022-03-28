<template>
  <div class="footer">
    <h1>{{ text }}</h1>
  </div>
</template>
<script>
export default {
  name: 'Footer',
  props: {
    text: {
      type: String,
    },
  },
};
</script>
<style scoped></style>
