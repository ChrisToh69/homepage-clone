<template>
  <div>
    <button class="btnstyle">{{ btnText }}</button>
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
.btnstyle {
  background-color: #d9534f; 
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  text-transform: uppercase;
  font-weight: bold;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.btnstyle:hover {
  background-color: #c9302c; /* Slightly darker on hover */
}
</style>