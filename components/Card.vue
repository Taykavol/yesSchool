<template>
  <div class="cardEng text-center border-2 my-8 py-8   mb-4">
      <div class="picture">
          <img alt="" :src="src" class="picture__image w-auto ">
      </div>
      <div class=" text-2xl text-green-700">Английский для детей</div>
      <div class=" text-sm">Приходите к нам на занятие</div>
  </div>
</template>

<script>
export default {
    props:{
        src:{
            type:String,
            require:true
        }
    }
}
</script>

<style lang="scss">
.picture {
    &__image {
        transition: all 1s; 
        
    }
    
}
.cardEng {
    width: 20rem;
    cursor: pointer;
    transition: all .5s;
    &:hover {
        transform: translateY(-.5rem);
    }
}
</style>