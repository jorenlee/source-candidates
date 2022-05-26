<template>
  <div>
    <Candidates/>
    <Posters/>
  </div>
</template>

<script>
  import Candidates from './components/Candidates.vue'
  import Posters from './components/Posters.vue'

export default {
  name: 'App',
  components: { 
    Candidates,
    Posters
  },
  data() {
    return {
  
    }
  }
}
</script>

<style>

</style>
