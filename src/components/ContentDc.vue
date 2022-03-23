<template>
    <div>
        <div class="container-black">
            inserisci qui il contenuto
        </div>
        <div class="container-blue">
            <ul>
                <li v-for="(card, index) in links" :key="index">
                    <a :href="card.href">
                        <img :src="card.icon" alt="">
                        <span>{{card.text}}</span>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import card1 from '../img/buy-comics-digital-comics.png'
import card2 from '../img/buy-comics-merchandise.png'
import card3 from '../img/buy-comics-subscriptions.png'
import card4 from '../img/buy-comics-shop-locator.png'
import card5 from '../img/buy-dc-power-visa.svg'

export default {
  name: 'ContentDc',
  data () {
      return{
          links: [
              {
                  href: '#',
                  icon: card1,
                  text: 'Digital Comics'
              },
              {
                  href: '#',
                  icon: card2,
                  text: 'Dc Merchandise'
              },
              {
                  href: '#',
                  icon: card3,
                  text: 'Subscription'
              },
              {
                  href: '#',
                  icon: card4,
                  text: 'Comic Shop location'
              },
              {
                  href: '#',
                  icon: card5,
                  text: 'Dc power Visa'
              },
          ]
      }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/css/style.scss';

.container-black{
    height: 200px;
    background-color: $black;
    color: $white;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container-blue{
    width: 99vw;
    height: 200px;
    background-color: $blue-DC;
    color: $white;
    display: flex;
    justify-content: center;
}

ul{
    width: 60%;
    list-style: none;
    display: flex;
    align-items: center;
    li{
        padding-right: 5rem;
        cursor: pointer;
    }
    a{
        text-decoration: none;
        size: 1rem;
        display: flex;
        justify-content: center;
        align-items: center;
        span{
            font-size: .8rem;
            padding-left: .5rem;
            text-transform: uppercase;
            color: $white;
        }
        img{
            width: 50px;
        }
    }
}

</style>

