<template>
  <div id="app">
    <div class="wrapper">
      <Header></Header>
      <div class="wrapper-content">
        <navigation></navigation>

        <div class="constent-wrapper">
          <!-- <contentproj v-for="(itam, index) in calc" :key="item[index]"></contentproj> -->
          <contentItem></contentItem>
          <contentItem></contentItem>
          <contentItem></contentItem>
          <a href="#" class="free-point">
            <img src="https://img.icons8.com/material/24/000000/new-moon--v1.png"/>
            <img src="https://img.icons8.com/material/24/000000/new-moon--v1.png"/>
            <img src="https://img.icons8.com/material/24/000000/new-moon--v1.png"/>
          </a>
        </div>
      </div>
      <div class="string_number">
        <a href="#">
          <img src="https://img.icons8.com/metro/26/000000/long-arrow-left.png"/>
        </a>
        <span>
          1 Страница
        </span>
        <a href="#">
          <img src="https://img.icons8.com/metro/26/000000/long-arrow-right.png"/>
        </a>
      </div>
      <Footer></Footer>
    </div>
  </div>
</template>
<script>
import Header from './components/Header.vue'
import navigation from './components/navigation.vue'
import contentItem from './components/contentItem.vue'
import Footer from './components/Footer.vue'

export default {
  name: "App",
  components: {
    Header,
    navigation,
    contentItem,
    Footer
  },
  data() {
    return{
      calc: 1
    }
  }
}
</script>

<style lang="scss">
#app {

  .wrapper{
  margin-right: auto; /* 1 */
  margin-left:  auto; /* 1 */
  display: flex;
  flex-direction: column;


  max-width: 1100px; /* 2 */





  .wrapper-content{
    width: 960px;
    align-self: center;

    .constent-wrapper{
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 50px;

    .free-point{
      display: flex;
      margin-top: 20px;

      img{
        width: 10px;
        height: 10px;
      }
    }

    }
    
  }
        .string_number{
        padding-top: 300px;
        display: flex;
        justify-content: center;
        align-items: center;
        line-height: 10px;

        span{
          margin: 0px 5px;
        }

        align-self: center;
      }
  }
}
</style>
