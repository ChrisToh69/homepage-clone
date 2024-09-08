<template>
    <div class="bg-gray-900 text-white relative flex items-center justify-center h-[480rem] max-h-[570px] min-h-full overflow-hidden z-0">
      <div class="w-full h-full self-center">
        <div class="flex justify-center mb-4 absolute w-full h-full top-0 left-0 ">
          <img src="/images/Banner1-jpg.webp" alt="Candles" class="w-full h-auto object-cover">
        </div>
        <div class="flex p-20 rounded-lg w-full h-full z-10 relative flex-col justify-center  bg-[#1f29374d] left-0">
          <p class="mb-4 border-white border-l-2 p-2 font-bold text-4xl">进口及本地各种神料用品</p>
          <simpleButton :btn-text="btnText" class=""/>
        </div>
      </div>
    </div>
</template>
  
<script>
import simpleButton from './ui/simple-button.vue';
export default {
  components: {
    simpleButton,
  },  
    data(){
    return{
      btnText:"理解更多",
    }
  }

  };
  </script>
  
  <style scoped>
  /* Add any additional custom styles here */
  </style>