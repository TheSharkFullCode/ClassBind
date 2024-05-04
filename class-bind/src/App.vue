

<template>

  <img alt="Vue logo" src="./assets/logo.png">
  <hr>

  <ClassBind/>
  <hr>
  <div class="Stylos">

    <span>Ciclo de vida de un componente, create{},  cuando el componente es creado, mount{}, cuando el componente es montado y update{}, cuando queremos que sucedan todas las actualizaciones</span>
  </div>

  <ClassOption/>
  
</template>



<script lang="ts" setup>

import ClassBind from "./components/ClassBind.vue";
import ClassOption from "./components/ClassOption.vue";

</script>

<style scoped>
.Stylos{
  border: 1px;
  border: black solid;
  border-radius: 3px;
  padding:  10px;
  background-color: aquamarine;
}
</style>
