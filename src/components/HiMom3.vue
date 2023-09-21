<script setup lang="ts">
function onClick(event: Event) {
  alert(`Hello Mom!`);
}

function onClick2(event: Event) {
  const clickedButton = event.currentTarget as HTMLButtonElement;
  alert(`${clickedButton.name} was clicked!`);
}
</script>
<template>
  <!--v-on:click= = :click this directive is used to set onclick event listener for a HTML element-->
  <button type="button" @click="onClick">Say Hello!</button>
  <button type="button" name="hiButton" @click="onClick2">Say Hi!</button>
</template>
