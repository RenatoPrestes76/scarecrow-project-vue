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
        <Title text="I have bad news for you" />
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

* {
  margin: 0%;
  padding: 0%;
}
body {
  width: 100%;
  height: 100vh;
}
main{
  display: flex;
  flex-direction: column;
}
.content {
  display: flex;
  flex-direction: row;
}
.left {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 50%;
  height: 70vh;
}
.img {
  display: flex;
  justify-content: center;
  align-items: center;
}
.scarecrow-img {
  display: flex;
  width: 35vw;
  min-width: 460px;
}

.right {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  width: 50%;
  height: 70vh;
}
.footer {
  width: 100%;
}
@media screen and (max-width: 1250px) {
  main {
    justify-content: start;
    gap: 10%;
  }
  .scarecrow-img {
    min-width: 260px;
    margin-left: -10%;
  }
  .content {
    flex-direction: column;
    width: 100%;
    gap: 30px;
  }
  .left {
    width: 100%;
    height: auto;
  }
  .right {
    width: 100%;
  }
}
</style>
