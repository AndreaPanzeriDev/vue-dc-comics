<template>
  <div class="card">
    <img :src="singleItem.thumb" alt="magazine  photo">
    <h6>{{singleItem.series}}</h6>
  </div>
</template>

<script>
export default {
    props:{
       singleItem: Object,
    }
}
</script>

<style scoped>
.card{
    width: calc(100% / 6);
}



h6{
    color: white;
    text-align: center;
}
</style>