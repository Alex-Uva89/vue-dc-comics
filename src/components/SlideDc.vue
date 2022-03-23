<template>
  <div class="card">
      <div class="container-img">
        <img :src="cardSrc" :alt="cardTitle">
      </div>
      <h2>{{ cardTitle }}</h2>
  </div>
</template>

<script>
export default {
    name: 'SlideDc',
    props: {
        cardSrc: String,
        cardTitle: String,
        cardPrice: String
    }
}
</script>

<style scope lang="scss">
@import '../assets/css/style.scss';

.card{
    width: calc(100% / 6);
    height: 180px;
    margin-bottom:1.5rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
    
    .container-img{
        width: 150px;
        height: 150px;
        overflow: hidden;
    }
    
    h2{
        text-transform: uppercase;
        font-size: .7rem;
    }
}
</style>