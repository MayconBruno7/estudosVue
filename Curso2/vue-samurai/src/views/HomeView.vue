<template>
  <b-container> 
    <b-row align-v="center">
      <BaseCard v-for="curso in cursos" :key="curso.id" :nome="curso.name" class="mb-5"></BaseCard>
    </b-row>
  </b-container>
</template>

<script>

import BaseCard from '@/components/BaseCard.vue'

export default {
  name: 'HomeView',
  data() {
    return {
      cursos: []
    }
  },  
  components: {
    BaseCard
  },
  mounted() {
    this.fetchData();
  },
  methods: {
    async fetchData() {
      const rest = await fetch("cursos.json");
      const val  = await rest.json();
      this.cursos = val
      console.log(val)
    }
  }
}
</script>
