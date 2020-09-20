<template>
  <div class="navigation">
    <div class="navigation-logo">
      <a href="#">
      </a>
    </div>
    <div class="navigation-breadcrumbs">
      <button>first</button>
      <button>second</button>
      <button>third</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navigation',
  props: {

  }
}
</script>


<style scoped lang="scss">
.navigation{


  &-logo{
    margin: 30px auto;
    display: flex;
    justify-content: center;

    a{
      width: 500px;
      height: 250px;
      background-image: url(../img/img-header/Logo2hightFinal.png);
      background-size: 500px;
      margin: 5px;
    }
  }
  &-breadcrumbs{
    display: flex;
    justify-content: center;

    button{
      width: 60px;
      height: 40px;
      margin: 5px;
    }
  }
}
</style>
