<template>
<div class="item">
  <img class="item_photo" src="../img/img-header/unnamed.png">
  <div class="item_right">
    <span class="item-title">Новость</span>
    <div class="item-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Saepe,
      culpa vero? Eaque necessitatibus illo dicta ex corrupti alias excepturi. Temporibus officiis
      quibusdam corporis accusamus, nostrum laborum illum laudantium recusandae ullam.
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'contentItem',
  props: {
    
  }
}
</script>

<style scoped lang="scss">
.item{
  padding: 20px;
  max-width: 500px;
  max-height: auto;
  display: flex;
  padding: 10px;
  border: 1px solid silver;
  margin: 5px;

  &_photo{
    width: 150px;
    height: 150px;
    padding-right: 8px
  }
  &-title{
    font-size: 20px;
    font-weight: 700;
  }
}
</style>