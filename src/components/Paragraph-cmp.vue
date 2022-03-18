<template>

  <div class="paragraph">
    <p>{{text}}</p>
  </div>
</template>
<script>
export default {
  name: 'Paragraph',
  props:{
    text:{
      type: String
    }
  }
};
</script>
<style scoped>
.paragraph p {
  font-family: 'Space Mono';
  font-style: normal;
  font-weight: 400;
  font-size: 30px;
  line-height: 35px;
  letter-spacing: -0.035em;
  color: #4f4f4f;
  width: 70%;
  margin: 0%;
}
@media screen and (max-width: 1250px) {
  .paragraph {
    display: flex;
    justify-content: center;
  }
  .paragraph p {
    width: 91%;
    font-size: 18px;
  }
}
</style>