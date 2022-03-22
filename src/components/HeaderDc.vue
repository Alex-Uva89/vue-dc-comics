<template>
  <header>
      <img alt="Dc logo" src="../img/dc-logo.png">
      <nav>
        <ul>
          <li @mouseover="setActiveIndex(index)"  v-for="(link, index) in links" :key="index" :class="{active: index == activeIndex}"><a :href="link.href"> {{link.text}} </a></li>
        </ul>
      </nav>
  </header>
</template>

<script>

export default {
  name: 'HeaderDc',
  data () {
    return {
      activeIndex: 0,
      links: [
        {
          href: '#',
          text: 'characters'
        },
        {
          href: '#',
          text: 'contacts'
        }, 
        {
          href: '#',
          text: 'tv'
        },
        {
          href: '#',
          text: 'movies'
        },
        {
          href: '#',
          text: 'games'
        },
        {
          href: '#',
          text: 'videos'
        },
        {
          href: '#',
          text: 'collectibles'
        },
        {
          href: '#',
          text: 'fans'
        },
        {
          href: '#',
          text: 'news'
        },
        {
          href: '#',
          text: 'shop'
        }
      ]
    }
  },
  methods:{
    setActiveIndex (index) {
      this.activeIndex = index
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/css/style.scss';

header{
  display: flex;
  justify-content: space-around;
  align-items: center;
}

li{
  display: inline-block;
  padding: 3rem 0rem 3rem;
  margin: 0 .5rem;
  &.active {
    color: $blue-DC;
    border-bottom: 5px solid $blue-DC
  }
  

  a {
    text-decoration: none;
    color: $black-text;
    
    &:hover {
      color: $blue-DC
    }
  }
  
}

</style>

