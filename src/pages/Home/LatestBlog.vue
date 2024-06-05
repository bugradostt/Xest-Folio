<template>
  <div class="body text-white">


    <div class="q-ma-xl">


      <div class="container">
        <div>
          <label class="title-blog">LatestBlog</label>
          <div class="des">Check Some of Latest
            <br>
          New & Articles

          </div>
        </div>
        <div>
          <div>Load More</div>
        </div>

      </div>


      <div class="row" v-for="i in 3" >

        <div class="col-md-2"></div>

        <div class=" col-sm-12 col-md-4">

          <CardBlog
          overline="UI Design  |   22 May  2023"
          title="test"
          img="/img/blog1.jpg"
          des="But I must explain to you how all this mistaken idea of denouncing pleasure and praising pain was born and I will give you a complete account of the system"
          >
          </CardBlog>

        </div>

        <div class=" col-sm-12 col-md-4">

        <CardBlog
        overline="UI Design  |   22 May  2023"
        title="test"
        img="/img/blog2.jpg"
        des="But I must explain to you how all this mistaken idea of denouncing pleasure and praising pain was born and I will give you a complete account of the system"
        >
        </CardBlog>

        </div>

        <div class="col-md-2"></div>

      </div>




    </div>
  </div>
</template>

<script setup>
import { ref  } from 'vue'
import CardBlog from 'src/components/CardBlog.vue'



</script>

<style scoped>


.body{
  background-color: #181818;
}

.container {
    display: flex;
    justify-content: space-between;
  }
  .title-blog {
    background: linear-gradient(90deg, #5635dd, #e63573);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
.des{
  font-size: 40px;
  font-weight: bold;
  line-height: 43px;

}
</style>

