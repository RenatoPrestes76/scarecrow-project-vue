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
<style scoped></style>
