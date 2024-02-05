<template>
    <div>
        <DestCard v-for="destination in destination" :key="destination.name" :Destination="destination"/>>
        <img :src="Destination.img" alt="">
        <h2>{{ Destination.name }}</h2>
        <h3>{{ Clicked }}</h3>
        <button @clicked="increment">Click Me</button>
    </div>
</template>

<script setup>
import { ref } from "vue";
const props = defineProps({
    Destination: Object,
});

const clicked = ref(0);
function increment() {
    clicked++;
}
</script>



<style scoped>

</style>
