<template>
  <div class="footer">
    <h1> {{text}}</h1>
  </div>
</template>
<script>
export default {
  name: 'Footer',
  props:{
    text:{
      type: String
    }
  }
};
</script>
<style scoped>
.footer {
  position: absolute;
  bottom: 0;
}
h1 {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  text-align: center;
  color: #bdbdbd;
}
@media screen and (max-width: 1250px) {
  .footer{
    position: relative;
  }
}
</style>