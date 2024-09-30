<template>
  <div>
      <Header />
      <floatingButton />
      <banner1 />
      <banner2 />
      <section1 />
      <simplebutton :btn-text="btnText" class="flex justify-center"/>
      <section2 />

    <Footer />
  </div>
</template>

<script>
import './index.css';
import Header from './components/layout/header.vue';
import Footer from './components/layout/footer.vue';
import banner1 from './components/banner1.vue';
import banner2 from './components/banner2.vue';
import section1 from './components/section/section1.vue';
import simplebutton from './components/ui/simple-button.vue';
import section2 from './components/section/section2.vue';
import floatingButton from './components/ui/floating-button.vue';

export default{
  components: {
    Header,
    Footer,
    banner1,
    banner2,
    section1,
    simplebutton,
    section2,
    floatingButton,
  },
  data(){
    return{
      btnText:"理解更多",
    }
  }
};

</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
