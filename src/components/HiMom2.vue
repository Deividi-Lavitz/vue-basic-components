<script setup lang="ts">
const name = 'Terezinha';
</script>
<template>
  <h2>Hi {{ name }}!</h2>
  <!--v-bind:datetime = :datetime this directive is used to set the attributes of a HTML element-->
  <p>
    It's <time :datetime="Date()">{{ new Date().toLocaleTimeString() }} </time>!
  </p>
</template>
