<template>
  <main>
    <Header text="404 not found" />
    <div class="content">
      <div class="left">
        <div class="img">
          <img class="scarecrow-img" src="./assets/Scarecrow.png" alt="Scarecrow" />
        </div>
      </div>
      <div class="right">
        <Title :level="1">I have bad news for you</Title>
        <Paragraph text=" The page you are looking for might be removed or is temporarily unavailable." />
        <Button text="BACK TO HOMEPAGE" />
      </div>
    </div>
    <div class="footer">
      <Footer text="created by <b>Prestes</b> - devChallenges.io" />
    </div>
  </main>
</template>
<script>
import Header from '@/components/Header-cmp.vue';
import Title from '@/components/Title-cmp.vue';
import Paragraph from '@/components/Paragraph-cmp.vue';
import Button from '@/components/Button-cmp.vue';
import Footer from '@/components/Footer-cmp.vue';


export default {
  name: 'App',
  components: {
    Header,
    Title,
    Paragraph,
    Button,
    Footer,
  },
};
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inconsolata:wght@700&display=swap');

@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&display=swap');

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@700&display=swap');


body {
  width: 100%;
  height: 100vh;
}
main{
  display: flex;
  flex-direction: column;
  margin: 0%;
}
.content {
  display: flex;
  flex-direction: start;
  justify-content: space-evenly;
}
.left {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 50%;
  height: 85vh;
}
.img {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.scarecrow-img {
  width: 28%;
  min-width: 460px;
}

.right {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  width: 50%;
  height: 85vh;
  margin: 0;
}
.footer {
  width: 100%;
}
@media screen and (max-width: 1250px) {
  main {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: flex-start;
    margin: 0%;
  }
  .content {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 90%;
    margin: 10%;
    gap: 30px;
  }
  .scarecrow-img {
    display: flex;
    flex-direction: row;
    align-content: center;
    width: 70vw;
    min-width: 160px;
  }
    .left {
    width: 75vw;
    height: 20vh;
  
  }
  .right {
    width: 90vw;
    height: 56vh;
    margin: 0%;
  }

}
</style>
