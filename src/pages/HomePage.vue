<template>
  <div>
    <div class="container constrain">
        <div class="column items-center sketch">
          <h1>Sketch</h1>
        </div>
        <div class="column items-center ink">
          <h1>Ink</h1>
        </div>
        <div class="column items-center colour">
          <h1>Color</h1>
        </div>
      </div>
        <div class="column items-center q-mt-xl">
          <q-btn
            to="/draw"
            size="xl"
            color="teal"
            label="Let's Draw!"
          />
        </div>>
  </div>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

<style lang="sass">

h1
  line-height: 20px

.sketch
  font-family: 'Londrina Sketch', cursive 
  background: white
  -webkit-background-clip: text
  -webkit-text-fill-color: transparent

.ink
  font-family: 'Dancing Script', cursive

.colour
  font-family: 'Sigmar One', cursive
  background: linear-gradient(to left, violet, indigo, blue, green, yellow, orange, red)
  -webkit-background-clip: text
  -webkit-text-fill-color: transparent
  

</style>