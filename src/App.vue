<template>
  <div>
    <LikeHeader></LikeHeader>
    <h2>{{ number }}</h2>
    <LikeNumber :total-number="number" v-on:my-click="number = $event"></LikeNumber>
    <LikeNumber :total-number="number"></LikeNumber>
  </div>
</template>

<script>
import LikeHeader from './components/LikeHeader.vue'

export default {
  data(){
    return{
      number:18
    };
  },
  components:{
    LikeHeader
  }
}
</script>

<style scoped>
div{
  border: 1px solid blue;
}
</style>