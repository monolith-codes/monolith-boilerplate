<template>
  <div class="home">
    <ProductionMaintenance />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ProductionMaintenance from "@/monolith/DefaultComponents/ProductionMaintenance.vue"; // @ is an alias to /src

export default defineComponent({
  name: "HomeView",
  components: {
    ProductionMaintenance,
  },
});
</script>

<style>
.home {
  background-color: red;
}
</style>
