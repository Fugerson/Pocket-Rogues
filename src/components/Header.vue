<template>
  <header class="header">
      <div class="header-left">
        <button class="some">some</button>
        <button class="some">some</button>
        <button class="some">some</button>
        <button class="some">some</button>
      </div>
      <div class="header-right">
        <div class="chenge_language">
          <a class="chenge_language-rus" href="#">
          </a>
          <a class="chenge_language-unit" href="#">
          </a>
        </div>
      </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {

  }
}
</script>


<style scoped lang="scss">
.header-wrapper{
}


.header{
height: 75px;
display: flex;
justify-content: space-between;
align-items: center;
position: sticky;
top: 0;
background: linear-gradient(0.25turn, #000000, #3f0f11, #9b1111);


  &-left{
    display: flex;


    button{
      width: 60px;
      height: 40px;
      margin: 5px;
    }
  }

  &-right{


    .chenge_language{
    display: flex;
    align-items: center;

      &-rus{
        width: 35px;
        height: 35px;
        background-image: url(https://img.icons8.com/emoji/48/000000/russia-emoji.png);
        background-size: 35px;
        margin: 5px;
      }
      &-unit{
        width: 35px;
        height: 35px;
        background-image: url(https://img.icons8.com/emoji/48/000000/united-kingdom-emoji.png);
        background-size: 35px;
        margin: 5px;
      }
    }
  }
}



</style>
