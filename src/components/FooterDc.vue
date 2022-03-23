<template>
<footer>
  <div class="container-footer">
      <div class="container-lists">
        <ul class="list">
            <li><h3>Dc Comics</h3></li>
            <li v-for="(link, index) in Comics" :key="index"><a :href="link.href">{{ link.text }}</a></li>
        </ul>
        <ul class="list">
            <li><h3>Shop</h3></li>
            <li v-for="(link, index) in shop" :key="index"><a :href="link.href">{{ link.text }}</a></li>
        </ul>
        <ul class="list">
            <li><h3>Dc</h3></li>
            <li v-for="(link, index) in dc" :key="index"><a :href="link.href">{{ link.text }}</a></li>
        </ul>
        <ul class="list">
            <li><h3>Sites</h3></li>
            <li v-for="(link, index) in sites" :key="index"><a :href="link.href">{{ link.text }}</a></li>
        </ul>
      </div>

      <div>
          <img src="../img/dc-logo-bg.png" alt="">
      </div>
  </div> 
  <!-- container fine -->
  <div class="container-bottom">
        <button>Sign-up</button>
        <ul class="list">
           <li>follow us</li>
           <li>
               <img src="../img/footer-facebook.png" alt="Facebook">
           </li>
           <li>
               <img src="../img/footer-periscope.png" alt="Periscope">
           </li>
           <li>
               <img src="../img/footer-pinterest.png" alt="Pinterest">
           </li>
           <li>
               <img src="../img/footer-twitter.png" alt="Twitter">
           </li>
           <li>
               <img src="../img/footer-youtube.png" alt="Toutube">
           </li>
        </ul>
  </div>
    
</footer>
</template>

<script>


export default {
    name: 'FooterDc',
    data (){
        return {
            Comics: [
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Movie'
                },
                {
                href: '#',
                text: 'Tv'
                },
                {
                href: '#',
                text: 'Games'
                },
                {
                href: '#',
                text: 'Videos'
                },
                {
                href: '#',
                text: 'News'
                }
            ],
            dc: [
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Comics'
                },
            ],
            sites: [
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
                {
                href: '#',
                text: 'Movie'
                },
                {
                href: '#',
                text: 'Tv'
                },
                {
                href: '#',
                text: 'Games'
                },
                {
                href: '#',
                text: 'Videos'
                },
                {
                href: '#',
                text: 'News'
                }
            ],
            shop: [
                {
                href: '#',
                text: 'Characters'
                },
                {
                href: '#',
                text: 'Comics'
                },
            ],
            // icons: [
            //     {
            //         image: 
            //     }
            // ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/css/style.scss';

.container-footer{
    height: 500px;
    color: $white;
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-image: url(../img/footer-bg.jpg);
    background-size: cover;
    overflow: hidden;
}

.container-lists{
    height: 70%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}

.list{
    margin-right: 1rem;
    margin-bottom: .6rem;
    list-style: none;
    li{
        margin: .2rem;
        h3{
            font-size: 1.1rem;
            text-transform: uppercase;
        }
        a{
            color: $white-text;
            text-decoration: none;
            &:hover{
                color: $white;
            }
        }
    }
}

.container-bottom{
    height: 100px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    background-color: $color-footer;
    button{
        cursor: pointer;
        font-weight: bold;
        text-transform: uppercase;
        padding: .8rem 1.5rem;
        color: $white;
        background-color: $transparent;
        border: 2px solid $white;
        &:hover{
            color: $black-text;
            background-color: $white;
            box-shadow: inset 0 0 5px $black;
            border: 1px solid $black;
            transition: all 1s;
        }
    }
    .list{
        font-weight: bold;
        text-transform: uppercase;
        color: $blue-DC;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 10px;
        img{
            cursor: pointer;
            &:hover{
                transform: scale(1.1);
                filter: brightness(100); 
                

            }
        }
    }
}


</style>