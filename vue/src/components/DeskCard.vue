<template>
  <div>
    <h1>Toppings</h1>
    <h2>{{ Destination.name }}</h2>
    <img :src="Destination.img" alt="Destination.name" />
    <h3>{{ clicked }}</h3>
    <button @click="increment">Click Me</button>
  </div>
</template>

<script setup>
let list = []
import { ref } from "vue";
const props = defineProps({
  Destination: Object,
});

//clicker logic
let clicked = ref(0);
function increment() {
  clicked.value++;
  list.push(props.Destination.name);
  console.log(list);
}
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin: 10px;
}

img {
  width: 250px;
  height: 300px;
  object-fit: cover;
}
</style>