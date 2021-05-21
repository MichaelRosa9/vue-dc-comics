<template>
  <main>

  <div class="container flex-between wrap">
    <Card v-for="(comic, index) in Comics" :key="index" 
      :card="comic" class="card"
    />
  </div>
    
  <Button class="button" :button_text="text"/>
  </main>
</template>

<script>
import Comics from '@/assets/data/dc-comics.json';
import Card from './Card.vue';
import Button from '@/components/Button-blue.vue'

export default {
  name: 'Main',
  components: {
    Card,
    Button
  },
  data(){
    return{
      Comics,
      text: 'Load More'
    }
  }
}
</script>


<style scoped lang="scss">

@import '../assets/styles/vars.scss';

.card {
  flex-basis: calc(100% / 6);
}

.button {
  display: block;
  margin: 50px auto 0;
  padding: 15px 65px;       
  box-shadow: 0 0 2px #000000;
  font-size: 12px;
}

</style>
