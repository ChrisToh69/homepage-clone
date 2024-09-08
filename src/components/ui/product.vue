<template>
  <div class="relative w-full h-full">
    <!-- Background Image -->
    <div
      class="absolute w-full h-full inset-0 bg-cover bg-center"
      :style="{ backgroundImage: `url('${cardDisplay.backgroundImage}')` }"
    ></div>

    <!-- Icon and Text Overlay -->
    <div class="absolute inset-0 flex flex-col justify-end p-4 text-white">
      <!-- Icon -->
      <div>
        <img :src="cardDisplay.icon" alt="Icon" class="w-8 h-8 mb-2" />
      </div>
      <!-- Text -->
      <div class="font-semibold text-xl">{{ cardDisplay.text }}</div>
    </div>
  </div>
</template>

<script>
export default {
    props: {
    cardDisplay: {
      type: Object,
      default: {
            backgroundImage: "",
            icon: "",
            text: ""
        }
    },
}, 
}
</script>

<style>

</style>