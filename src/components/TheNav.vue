<template>
<div class="navContainer">
        <li @click="increment('TEST')">Oplysninger</li>
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

<script>
export default {
  data() {
    return {
      count: 1
    }
  },
  methods: {
    increment() {
      this.count++
      console.log(this.count)
    }
  }
}
</script>
