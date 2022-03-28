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
<style scoped></style>
