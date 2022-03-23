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
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0;
    &:hover{
                padding: .5rem;
                transform: scale(1.3);
                background-color: $blue-DC;
                align-items: center;
                z-index: 5;
                border-radius: 1rem;
                transition: padding 1s, transform 1.5s, background-color 1s, align-items 1.5s, z-index 1.5s;
            }
    .container-img{
        width: 150px;
        height: 150px;
        overflow: hidden;
        position: relative;
        margin-bottom: 5px;
        &:hover{
            border-radius: 1rem;
        }
        img{
            width: 105%;
            position: absolute;
            top:0;
            right: 0%;
        }
    }
    
    h2{
        text-transform: uppercase;
        font-size: .7rem;
    }
}
</style>