<template>
  <div class="footer">
    <h1>{{ texto }}</h1>
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
