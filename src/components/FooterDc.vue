<template>
  <div class="container-footer">
      <ul>
          <li>
              Dc Comics
              <ul>
                  <li v-for="(item, index) in item" :key="index">{{item}}</li>
              </ul>
          </li>
          <li>
              Dc Comics
              <ul>
                  <li v-for="(item, index) in item" :key="index">ciao</li>
              </ul>
          </li>
          <li>
              Dc Comics
              <ul>
                  <li v-for="(item, index) in item" :key="index">ciao</li>
              </ul>
          </li>
          <li>
              Dc Comics
              <ul>
                  <li v-for="(item, index) in item" :key="index">ciao</li>
              </ul>
          </li>
      </ul>
      <div>
          <img src="../img/dc-logo-bg.png" alt="">
      </div>
  </div>
</template>

<script>
export default {
    name: 'FooterDc',
    data (){
        return {
            items: [
                {
                    item:[
                        'uno',
                        'due',
                        'tre',
                        'quattro',
                        'cinque',
                        'sei',
                        'sette',
                        'otto',
                        'nove',
                     ]

                },
                {
                    item:[
                        'uno',
                        'due',
                        'tre',
                        'quattro',
                        'cinque',
                        'sei',
                        'sette',
                        'otto',
                        'nove',
                     ]
                },
                {
                    item:[
                        'uno',
                        'due',
                        'tre',
                        'quattro',
                        'cinque',
                        'sei',
                        'sette',
                        'otto',
                        'nove',
                     ]
                },
                {
                    item:[
                        'uno',
                        'due',
                        'tre',
                        'quattro',
                        'cinque',
                        'sei',
                        'sette',
                        'otto',
                        'nove',
                     ]
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/css/style.scss';

.container-footer{
    height: 400px;
    width: 100vw;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    background-image: url(../img/footer-bg.jpg);
    background-size: cover;
    overflow: hidden;
}

li{
    color: $white;
}

</style>