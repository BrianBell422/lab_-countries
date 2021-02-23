<template lang="html">
  <div id="favourite_countries">
    <h2>Favourite Countries</h2>
    <li>{{ country }}</li>
  </div>
</template>

<script>
export default {
  name: 'favourite-countries',
  props: ['favourite-country']
}
</script>

<style lang="css" scoped>
</style>
