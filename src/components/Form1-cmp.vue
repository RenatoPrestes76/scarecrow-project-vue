<template>
  <div class="form1">
    <p>{{ text }}</p>
  </div>
</template>
<script>
export default {
  name: 'Form1',
  props: {
    text: {
      type: String,
    },
  },
};
</script>
<style scoped></style>
