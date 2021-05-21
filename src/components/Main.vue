<template>
  <main>

  <div class="container flex-between wrap">
    <Card v-for="(comic, index) in Comics" :key="index" 
      :card="comic" class="card"
    />
    
  </div>
    
  </main>
</template>

<script>
import Comics from '@/assets/data/dc-comics.json';

import Card from './Card.vue';

export default {
  name: 'Main',
  components: {
    Card
  },
  data(){
    return{
      Comics
    }
  }
}
</script>


<style scoped lang="scss">

@import '../assets/styles/vars.scss';

.card {
  flex-basis: calc(100% / 6);
}

</style>
