<template>
  <div class="container">
    <DestCard
      v-for="destination in destinations"
      :key="destination.name"
      :Destination="destination"
      @click="handleCardClick"
    />
  </div>
</template>

<script setup>
import DestCard from "@/components/DeskCard.vue";
import { ref } from "vue";


const destinations = [
  {
    name: "Black Beans",
    group: "Protien",
    calories: 130,
    price: 0,
    img: "https://media.istockphoto.com/id/693678298/photo/black-beans-on-white-background.jpg?s=612x612&w=0&k=20&c=MVsSvg84IEqDF-C0jPCK04EJCKLAzszHdDgWCM9MHA4=",
  },
  {
    name: "Pinto Beans",
    group: "Protien",
    calories: 130,
    price: 0,
    img: "https://media.istockphoto.com/id/172399182/photo/pinto-beans.jpg?s=612x612&w=0&k=20&c=BgN-h5nvUA8JoM45iLRUWMh8tJdhUQnZpip0_Gzm1bA=",
  },
  {
    name: "White Rice",
    group: "Grain",
    calories: 210,
    price: 0,
    img: "https://media.istockphoto.com/id/171552859/photo/white-basmati-rice.jpg?s=612x612&w=0&k=20&c=0MjDWXL4qr--uPT4llvQWZDR5p9jkKhnZgacuW1DBGM=",
  },
  {
    name: "Brown Rice",
    group: "Grain",
    calories: 210,
    price: 0,
    img: "https://media.istockphoto.com/id/1407028798/photo/brown-rice-on-white.jpg?s=612x612&w=0&k=20&c=YA-sMDlWucWk9gROZDACHqEWJOW7thH1NmRGxbo0Mng=",
  },
  {
    name: "Tomato Salsa",
    group: "Vegetable",
    calories: 25,
    price: 0,
    img: "https://media.istockphoto.com/id/117227395/photo/sauce.jpg?s=612x612&w=0&k=20&c=fKp4_rwGD-FoXL_kIV6VC__G4jSpAN3H9Z9D6V70fE8=",
  },
  {
    name: "Sweet Corn",
    group: "Vegetable",
    calories: 80,
    price: 0,
    img: "https://media.istockphoto.com/id/1222272368/photo/corn-seeds-3d-rendering.jpg?s=612x612&w=0&k=20&c=7YwA_g8h6zxbfZp-H_iPDu26yaZx5xpcK6GozeCUBUw=",
  },
  {
    name: "Cheese",
    group: "Dairy",
    calories: 110,
    price: 0,
    img: "https://media.istockphoto.com/id/117713098/photo/cheese-pile.jpg?s=612x612&w=0&k=20&c=JEwTiKop-dT3DPHCabJhx97efAej8vvDOw0tOD8jt0g=",
  },
  {
    name: "Sour Cream",
    group: "Dairy",
    calories: 110,
    price: 0,
    img: "https://media.istockphoto.com/id/1135483731/photo/sour-cream-or-yogurt-in-wooden-bowl.jpg?s=612x612&w=0&k=20&c=9CZ2DyG-3ZWeu-4802fbWGOIGVgt47CIlGCslMU8MxM=",
  },
  {
    name: "Lettuce",
    group: "Vegetable",
    calories: 5,
    price: 0,
    img: "https://media.istockphoto.com/id/1426635953/photo/heap-of-sliced-green-lettuce-isolated-on-white.webp?b=1&s=170667a&w=0&k=20&c=A8LOGN2V4ddu6Mh5ToQdkCwHSqSivDI4iat6y0o0a8Y=",
  },
  {
    name: "Chicken",
    group: "Protien",
    calories: 180,
    price: 0,
    img: "https://media.istockphoto.com/id/1327004846/photo/poultry-meat-chicken-breast-after-cooked-on-white-background.webp?b=1&s=170667a&w=0&k=20&c=_j9466WlH_OvyS6AH--Bn3chuRRfI6g4i8OM3Wo3tTU=",
  },
  {
    name: "Steak",
    group: "Protien",
    calories: 150,
    price: 0,
    img: "https://media.istockphoto.com/id/172477497/photo/roasted-pork-stripes.jpg?s=612x612&w=0&k=20&c=MRzHf6cR61zpDU_1iu2tVbl1bgAmANJzbYcW_jov6dY=",
  },
  {
    name: "Guacemole",
    group: "Vegetable",
    calories: 0,
    price: 0,
    img: "https://media.istockphoto.com/id/469866573/photo/guacamole-dip.jpg?s=612x612&w=0&k=20&c=OjXhn4jL5qVzyUtoBtzGL1g8OVzqrysmfzwHNjLcVc0=",
  },

];
// Array to store clicked card names
const clickedCards = ref([]);

// Function to handle card click event
function handleCardClick(cardName) {
  clickedCards.value.push(cardName);
  console.log(clickedCards.value);
}
</script>

<style scoped>
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center; 
  align-items: center; 
  gap: 20px; 
}
</style>