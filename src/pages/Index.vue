<template>
  <div class="q-pa-md q-gutter-sm">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
      <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
    </q-carousel>
    <div class="right">
      <q-btn icon="style" @click="$router.replace('/')"  to="/aboutme" label="About Me" outline color="green" />
  </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      slide: 1
    }
  }
}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
.borders
  border-style: solid
  border-color: green
  margin: 10px
.left
  margin: auto
.right
  margin: 40px 0px
  text-align: center
  width: 100%
</style>
