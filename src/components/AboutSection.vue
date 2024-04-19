<template>
  <div class="flex-tags">
    <div class="img_container"> <img src="@/assets/deadline.png" alt="posted logo" /> </div>
    <div>
      <p>{{ title }}</p>
      <p>{{ desc }}</p>
    </div>
  </div>
</template>


<script>
export default {
  props: {
    img:{
        type :String,
        default : ''
    },

    title: {
        type : String,
        default : ''
    },
    
    desc: {
        type : String,
        default : ''
    },
  },
};
</script>


<style>
.flex-tags {
  display: flex;
  align-items: center
};
.img_container{
  width:'50px';
  height : '50px';
  margin-right: 20;
}
</style>
