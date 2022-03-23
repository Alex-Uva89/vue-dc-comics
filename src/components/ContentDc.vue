<template>
    <main>
        <div class="container-black">
            <div class="container-slides">
            <button class="series-btn">current series</button>
            <SlideDc v-for="(card,index) in slides" 
            :key="index" 
            :card-src="card.thumb" 
            :card-price="card.price"
            :card-title="card.series" 
            class="card"
             />
            </div>

            <div class="container-btn">
                <button>load more</button>
            </div>
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
    </main>
</template>

<script>
import card1 from '../img/buy-comics-digital-comics.png'
import card2 from '../img/buy-comics-merchandise.png'
import card3 from '../img/buy-comics-subscriptions.png'
import card4 from '../img/buy-comics-shop-locator.png'
import card5 from '../img/buy-dc-power-visa.svg'
import SlideDc from './SlideDc.vue'

export default {
  name: 'ContentDc',
  components: {
      SlideDc
  },
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
          ],
        slides: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
]
      }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/css/style.scss';

.container-black{
    background-color: $black;
}

.container-slides{
    width: 1000px;
    margin: 0 auto;
    padding-top: 5rem;
    color: $white;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    position: relative;
    .series-btn{
        position: absolute;
        left: 0;
        top: -15px;
    }
}

.container-btn{
    width: 100%;
    height: 8rem;
    display: flex;
    justify-content: center;
    align-items: center;
}

button{
    color: $white;
    text-transform: uppercase;
    padding: .5rem 3rem;
    background-color: $blue-DC;
}


.container-blue{
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

