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
  display: flex;
  flex-direction: column;
  justify-items: center;
  align-content: flex-end;
}
h1 {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  text-align: center;
  color: #bdbdbd;
  margin: 0%;
}
@media screen and (max-width: 1250px) {
  .footer{
   display: flex;
   flex-direction: column;
   justify-content: space-evenly;
   align-items: flex-end;
  }
  h1 {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  text-align: center;
  color: #bdbdbd;
  margin: 0%;
}
}
</style>