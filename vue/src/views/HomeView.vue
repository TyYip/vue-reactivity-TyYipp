<template>
  <div>
    <DestCard
      v-for="destination in destinations"
      :key="destination.name"
      :Destination="destination"
    />
  </div>
</template>

<script setup>
import DestCard from "@/components/DeskCard.vue";
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
    calories: 130
    price: 0,
    img: "https://media.istockphoto.com/id/172399182/photo/pinto-beans.jpg?s=612x612&w=0&k=20&c=BgN-h5nvUA8JoM45iLRUWMh8tJdhUQnZpip0_Gzm1bA=",
  },
  {
    name: "White Rice",
    group: "Grain",
    calories: 210,
    price: 0,
    img: "https://images.unsplash.com/photo-1547138494-97041dec734b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1170&q=80&quot;",
  },
  {
    name: "Brown Rice",
    group: "Grain",
    calories: 210,
    price: 0,
    img: "https://images.unsplash.com/photo-1507525428034-b723cf961d3e?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1173&q=80&quot;",
  },
  {
    name: "Tomato Salsa",
    group: "Vegetable",
    calories: 25,
    price: 0,
    img: "https://images.unsplash.com/photo-1511497584788-876760111969?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1332&q=80&quot;",
  },
  {
    name: "Sweet Corn",
    group: "Vegetable",
    calories: 80,
    price: 0,
    img: "",
  },
  {
    name: "Sweet Corn",
    group: "Vegetable",
    calories: 80,
    price: 0,
    img: "",
  },
  {
    name: "Sweet Corn",
    group: "Vegetable",
    calories: 80,
    price: 0,
    img: "",
  },
  {
    name: "Sweet Corn",
    group: "Vegetable",
    calories: 80,
    price: 0,
    img: "",
  },
];
</script>

<style scoped></style>
