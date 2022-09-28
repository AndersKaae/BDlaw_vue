<script>
import Oplysninger from './Oplysninger.vue'
import Datapolitik from './Datapolitik.vue';
export default{
    components: { Oplysninger, Datapolitik },
    props: ['oplysningerDisplay','windowState'],
}

</script>
<template>
    <div class="content-container">
        <div v-if="windowState.oplysninger">
            <Oplysninger />
        </div>
        <div v-if="windowState.datapolitik">
            <Datapolitik />
        </div>
        <h1 v-cloak class="title">BD Law</h1>
      <h1 v-cloak class="tagline">LET'S GET LEGAL</h1>
    </div>
</template>

<style scoped>
.content-container{
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-color: transparent;
}
.title{
  font-family: "StickyPops", Helvetica, Arial;
  font-size: 200px;
  color: white;
  text-align: center;
}
.tagline{
  font-family: "StickyPops", Helvetica, Arial;
  font-size: 100px;
  color: white;
  padding-top: 100px;
  text-align: center;
}
</style>
