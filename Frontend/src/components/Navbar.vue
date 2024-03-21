<template>
  <header>
    <nav class="bg-transparent z-50">
      <div class="container mx-auto flex justify-between items-center h-16">
        <div class="flex items-center">
          <img :src="logo" alt="Logo" class="w-10 h-10" />
          <h1 class="text-black ml-2 font-bold">{{ empresa }}</h1>
        </div>
        <ul class="flex items-center">
          <li>
            <a :href="href1"
              class="text-black px-3 hover:bg-orange-400 hover:border-2 border-b-black rounded-md hover:text-white">{{
            texto1 }}</a>
          </li>
          <li>
            <a :href="href2"
              class="text-black px-3 hover:bg-orange-400 hover:border-2 border-b-black rounded-md hover:text-white">{{
            texto2 }}</a>
          </li>
          <li>
            <a :href="href3"
              class="text-black px-3 hover:bg-orange-400 hover:border-2 border-b-black rounded-md hover:text-white">{{
            texto3 }}</a>
          </li>
        </ul>
        <ButtonSingUp />
      </div>
    </nav>
  </header>
</template>

<script setup>
import { ref } from "vue";
import ButtonSingUp from "./ButtonSingInUp.vue";

const logo = ref("https://www.svgrepo.com/show/333609/tailwind-css.svg");
const empresa = ref("Nombre de la empresa");
const href1 = ref("#");
const texto1 = ref("Texto botón 1");
const href2 = ref("#");
const texto2 = ref("Texto botón 2");
const href3 = ref("#");
const texto3 = ref("Texto botón 3");
const login = ref("#");

//OPTIONS API
//export default {
//   setup() {
//     const logo = ref("https://www.svgrepo.com/show/333609/tailwind-css.svg");
//     const empresa = ref("Nombre de la empresa");
//     const href1 = ref("#");
//     const texto1 = ref("Texto botón 1");
//     const href2 = ref("#");
//     const texto2 = ref("Texto botón 2");
//     const href3 = ref("#");
//     const texto3 = ref("Texto botón 3");
//     const login = ref("#");

//     return {
//       logo,
//       empresa,
//       href1,
//       texto1,
//       href2,
//       texto2,
//       href3,
//       texto3,
//       login,
//     };
//   },
// };
</script>

<style>
.container {
  max-width: 1200px;
}
</style>
