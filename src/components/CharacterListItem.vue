<template lang="html">
  <div>
  <li>{{character.name}} Height: {{character.height | toMetres}}m</li>
</div>
</template>

<script>
export default {
  name: 'character-list-item',
  props: ['character'],
  filters: {
      toMetres: function(value){
        return value / 100
      }
    },
}
</script>

<style>
</style>
