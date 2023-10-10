<script >
export default{
  data() {
    return{
      
      slides: [
        "https://i0.wp.com/www.giacomocusano.com/wp-content/uploads/2016/07/coastal-wash-web.jpg?fit=1024%2C682&ssl=1",
        "https://www.artemedialab.it/wp-content/uploads/2019/04/immagini-sfondo-1-700x400.jpg",
        "https://fotografiaartistica.it/wp-content/uploads/2019/06/nasa-immagini-gratuite-dello-spazio.jpg"],
      
      
      
    };
    
  },
  methods:{
    imagedestra(){
      this.slides[0]
    }
  }
};
</script>

<template>
  <div class="arrows">
      <div class="arrows-left" >&#129044;</div>
      <div class="arrows-right" @click="imagedestra">&#129046;</div>
    </div>
 <div class="carousel">
      <img  v-for="slide in slides" :key="slide" :src="slides[0]">
 </div>
</template>

<style scoped>
.carousel{
  display: flex;
  align-content: center;
  
}
.arrows{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.arrows-left, .arrows-right{
  font-size: 100px;
}
</style>
