<template lang="pug">
  li.artist
    h2: a(:href="artist.url" target="_blank") {{ artist.name }}
    img(:src="artist.image[2]['#text']")
</template>

<script>
  export default {
    name: 'artist',
    props: [ 'artist' ]
  }
</script>

<style lang="stylus" scoped>
/* scoped = reduce el alcanze del css para que no pise estilos de otro componente*/
li.artist
  display block
  margin 10px 0
</style>