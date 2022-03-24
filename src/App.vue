<template>
  <main>
    <Header text="404 not found" />
    <div class="content">
      <div class="left">
        <div class="img">
          <img
            class="scarecrow-img"
            src="./assets/Scarecrow.png"
            alt="Scarecrow"
          />
        </div>
      </div>
      <div class="right">
        <Title :level="1">I have bad news for you</Title>
        <Paragraph
          text=" The page you are looking for might be removed or is temporarily unavailable."
        />
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
  margin: 0;
}
main {
  display: flex;
  flex-direction: column;
  margin: 0;
}
.content {
  display: flex;
  flex-direction: row;
  width: 85vw;
  height: 90vh;
  margin: 0;
}
.left {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  width: 100vw;
  height: 95%;
  margin: 0;
}
.img {
  max-width: 500px;
}
.scarecrow-img {
  display: flex;
  flex-direction: row;
  align-items: center;
  width: 100%;
  min-width: 400px;
}
.right {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: flex-start;
  width: 50%;
  height: 95%;
  margin: 0%;
}
.footer {
  width: 100%;
}
@media screen and (max-width: 1250px) {
  body {
    width: 100%;
    height: 100vh;
    margin: 0;
  }
  main {
    display: flex;
    flex-direction: column;
    margin: 0%;
  }
  .content {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    width: 100%;
    height: 100%;
    gap: 10px;
    margin: 0;
  }
  .left {
    display: flex;
    flex-direction: row;
    align-content: center;
    width: 100%;
    height: 100%;
    margin: 0;
  }
  .img {
    max-width: 250px;
  }
  .scarecrow-img {
    min-width: 160px;
  }
  .right {
    display: flex;
    width: 85vw;
    height: 45%;
    margin: 10%;
    gap: 30px;
  }
}
</style>
