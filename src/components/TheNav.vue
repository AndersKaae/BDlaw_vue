<script>
  export default {
    props: ['windowState'],
    emits: ['update:windowState'],
    methods: {
      toggleOpylsninger(type) {
        var data = this.windowState;
        if (type == 'oplysninger') {
          data.oplysninger =! data.oplysninger
        }
        if (type == 'datapolitik') {
          data.datapolitik =! data.datapolitik
        }
      this.$emit('update:windowState', data)
    },
    toggleDatapolitik(windowState) {
      windowState.datapolitik = !windowState.datapolitik
      this.$emit('update:windowState', windowState)
    }
  }
}
  </script>

<template>
<div class="navContainer">
        <li @click="toggleOpylsninger('oplysninger')">Oplysninger</li>
        <li @click="toggleOpylsninger('datapolitik')">Datapolitik</li>
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