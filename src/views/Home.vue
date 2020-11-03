<template>
  <div>
    <h1  @click="increaseCapacity()">My Event</h1>
    <p>Capacity: {{ capacity }}</p>
    <button  @click="capture()">Capture</button>
  </div>
</template>

<script>
import { ref } from "vue"; // <-- Use this line if you're in a Vue 3 app
export default {
  
  setup() {
    const capacity = ref(3);
    
    
    function increaseCapacity() { 
      console.log(capacity.value)
      capacity.value++;
    }
    return { capacity, increaseCapacity, capture };
  }
  
};
</script>

<style scoped>
p, h1{
  color:blue;
}
</style>