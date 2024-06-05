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



    </div>
  </div>
</template>

<script setup>
import { ref  } from 'vue'



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

