<script>
  import HeaderComponent from './components/HeaderComponent.vue';

  export default {
    components: {
      HeaderComponent,
    }
  }
</script>

<template>
  <div id="app">
    <HeaderComponent />
    <router-view/>
  </div>
</template>


