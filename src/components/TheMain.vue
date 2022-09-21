<script>
import Oplysninger from './Oplysninger.vue'
export default{
    components: { Oplysninger },
    props: ['oplysningerDisplay'],
}

</script>
<template>
    <div class="content-container">
        <div v-if="oplysningerDisplay">
            <Oplysninger />
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
