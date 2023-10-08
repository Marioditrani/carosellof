<script >
export default{
  data() {
    return{
      slides: [
        {
          id: 1,
          image: "https://i0.wp.com/www.giacomocusano.com/wp-content/uploads/2016/07/coastal-wash-web.jpg?fit=1024%2C682&ssl=1"
        },
        {
          id: 2,
          image: "https://www.artemedialab.it/wp-content/uploads/2019/04/immagini-sfondo-1-700x400.jpg"
        },
        {
          id: 3,
          image: "https://fotografiaartistica.it/wp-content/uploads/2019/06/nasa-immagini-gratuite-dello-spazio.jpg"
        },
      ],
    };
  },
  methods:{
    imageRight(){
      
    }
  }
};
</script>

<template>
  <div class="arrows">
      <div class="arrows-left" >&#129044;</div>
      <div class="arrows-right">&#129046;</div>
    </div>
 <div class="carousel">
    <div class="slide" v-for="slide in slides" :key="slide.id">
      <img :src="slide.image">
    </div>
    
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
