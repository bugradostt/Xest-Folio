<template>
  <div class="q-ma-xl body bg-white">

    <div class="container">
        <div>
          <label class="title-portfolio">PORTFOLIO</label>
          <div class="des">
            Some Of Our Best Works

          </div>
        </div>
        <div>



          <div>

            <div class="load-more">
              Load More
            </div>

            <div class="load-more-gradient">

          </div>



        </div>
        </div>

      </div>

      <div class="row">

        <div class="col-4" v-for="i in imgList">
          <Card :img="i"></Card>
        </div>





      </div>


  </div>
</template>

<script setup>
import Card from 'src/components/Card.vue'

var imgList = [
  "public/img/laptop.jpg",
  "public/img/laptop2.jpg",
  "public/img/kamera.jpg",
  "public/img/kamera.jpg",
  "public/img/laptop.jpg",
  "public/img/laptop2.jpg",
  "public/img/laptop.jpg",
  "public/img/laptop2.jpg",
  "public/img/kamera.jpg",
]

</script>

<style scoped>

.container {
    display: flex;
    justify-content: space-between;
  }
  .title-portfolio {
    background: linear-gradient(90deg, #5635dd, #e63573);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
.des{
  font-size: 30px;
  font-weight: bold;
  line-height: 43px;

}

.load-more {
    color: white;
    background-color: black;
    font-size: 12px;
    padding: 10px;
    position: relative;
    z-index: 2;
  }

  .load-more-gradient {
    padding: 15px;
    width: 100%;
    height: 100%;
    background-color: #5635dd;
    background-image: linear-gradient(90deg, #5635dd 0%, #e63573 100%);
    position: relative;
    margin-left:5px ;
    margin-top: -25px;
    z-index: 1;
  }

</style>

