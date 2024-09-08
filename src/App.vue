<template>
  <div>
    <Header />
    <banner1 />
    <banner2 />
    <section1 />
    <!-- <simplebutton :btn-text="btnText"/> -->
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


export default{
  components: {
    Header,
    Footer,
    banner1,
    banner2,
    section1,
    simplebutton,
  },
  data(){
    return{
      btnText:"asdf",
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
