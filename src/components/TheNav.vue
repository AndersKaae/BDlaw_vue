<script>
  export default {
    props: ['modelValue'],
    emits: ['update:modelValue'],
    methods: {
    toggleBox(modelValue) {
      modelValue = !modelValue
      this.$emit('update:modelValue', modelValue)
    }
  }
}
  </script>

<template>
<div class="navContainer">
        <li @click=toggleBox(modelValue)>Oplysninger</li>
        <li>Datapolitik</li>
        <li>Betingelser</li>
        <li>Kontakt</li>
</div>
</template>

<style scoped>
.navContainer {
    left: 0;
    width: 100vw;
    position: absolute;
    top: 10px;
    text-align: center;
    z-index: 10;
}
li {
    display: inline;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 20px;
    padding-right: 70px;
    color: rgb(208, 23, 222);
    font-weight: 800;
    cursor: pointer;
}
</style>