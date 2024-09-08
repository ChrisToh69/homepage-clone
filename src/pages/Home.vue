<script setup>
import { ref } from 'vue'
import Footer from '../components/layout/footer.vue';
import Banner1 from '../components/banner1.vue';

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <Banner1></Banner1>
  <Footer></Footer>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
