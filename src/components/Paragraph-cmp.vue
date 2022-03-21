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
  height: 18vh;
  margin: 0%;
}
@media screen and (max-width: 1250px) {
  .paragraph {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-end;
  }
  .paragraph p {
    font-family: 'Space Mono';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 25px;
    letter-spacing: -0.035em;
    color: #4f4f4f;
    width: 100%;
    height: 10vh;
    margin: 0%;    
  }
}
</style>