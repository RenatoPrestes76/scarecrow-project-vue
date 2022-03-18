<template>
  <div class="title">
    <h1>{{text}}</h1>
  </div>
</template>
<script>
export default {
  name: 'Title',
  props:{
    text:{
      type: String
    }
  }
};
</script>
<style scoped>
.title h1 {
  font-family: 'Space Mono';
  font-style: normal;
  font-weight: 700;
  font-size: 80px;
  line-height: 70px;
  letter-spacing: -0.035em;
  color: #333333;
  width: 50vw;
  height: 20vh;
  margin: 0%;
}
@media screen and (max-width: 1250px) {
  .title{
    display: flex;
    justify-content: flex-end;
    margin: 0%;
  }
  .title h1{
    width: 96%;
    font-size: 48px;
    margin: 0%;
  } 
}
</style>