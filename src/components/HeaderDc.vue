<template>
  <nav>
    <ul>
      <li v-for="(link, index) in links" :key="index"><a :href="link.href"> {{link.text}} </a></li>
    </ul>
  </nav>
</template>

<script>

export default {
  name: 'HeaderDc',
  data () {
    return{
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
  }
}
</script>

<style scoped lang="scss">
@import '../assets/css/style.scss';

li{
  display: inline-block;
  padding: .5rem;
  a {
    text-decoration: none;
    color: var(--black-text)
  } 
}

</style>

