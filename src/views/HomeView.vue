<script>
import { RouterView } from "vue-router";
import CarCeu from "@/components/CarCeu.vue";
import ListaDisp from "@/components/ListaDisp.vue";
import CardFilme from "../components/CardFilme.vue";

export default {
  components: { CarCeu, CardFilme, ListaDisp, RouterView },
};
</script>
<template>
  <RouterView />
  <CarCeu />
  <ListaDisp />
  <!-- <CardFilme /> -->
</template>
<style>
@import "@/assets/base.css";
</style>
