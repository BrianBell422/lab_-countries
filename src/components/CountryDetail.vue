<template lang="html">
  <div id="selected_country">
    <h2>Country Name: {{ country.name }}</h2>
    <p> Population: {{ country.population }}</p>
    
    <img class="lrg-flag" :src="country.flag"/>

    <neighbouring-countries>
    </neighbouring-countries>

</div>
</template>

<script>
import NeighbourCountry from './NeighbourCountry.vue';
export default {
  name: 'country-detail',
  props: ['country', 'country.flag'],
  components: {
    'neighbouring-countries': NeighbourCountry
  }
}
</script>

<style lang="css" scoped>

.lrg-flag {
  height: 100px
}

</style>
