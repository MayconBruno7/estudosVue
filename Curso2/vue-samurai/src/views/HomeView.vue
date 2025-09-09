<template>
  <b-container> 
    <b-row align-v="center">
      <BaseCard />
    </b-row>
  </b-container>
</template>

<script>
// @ is an alias to /src
import BaseCard from '@/components/BaseCard.vue'

export default {
  name: 'HomeView',
  components: {
    BaseCard
  }
}
</script>
