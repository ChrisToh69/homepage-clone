<template>
  <div>
    <button class="mt-[10px] bg-transparent border-red-500 py-2 px-4 rounded-full uppercase font-bold border-2 cursor-pointer transition duration-300 ease-in-out hover:bg-red-200">{{ btnText }}</button>
  </div>
</template>

<script>
export default {
  props: {
    btnText: String
  }
}
</script>

<style scoped>

</style>