<template>
  <div class="q-ma-xl">


    <div class="flex-container" >
      <div class="flex-item">

        <div class="miami">MIAMI</div>
        <div class="walker">
          WALKE<span style="color: white;">R</span>

        </div>
        <label class="des">Award Wining product designer based in Georgia. We
<br>
          create user-friendly interfaces for
          fast-growing startups.</label>

        <div>
          <br>

          <div class="book">
            Book A Call
          </div>

          <div class="book-gradient">

          </div>

        </div>

      </div>

      <div class="flex-item">
        <q-img src="/public/img/banner.jpg" class="img" />
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.img {
  width: 560px;
  border-radius: 0 50px 0 50px;
  z-index: 1;

}

.flex-container {
  display: flex;
  align-items: center;
  justify-content: center;

}

.flex-item {
  margin-right: 20px;

}

.flex-item:last-child {
  margin-right: 0;

}


.book {
    color: white;
    background-color: black;
    font-size: 12px;
    padding: 10px;
    position: relative;
    z-index: 2;
    width: 100px;
    text-align: center;
  }

  .book-gradient {
    padding: 15px;
    width: 100px;
    height: 100%;
    background-color: #5635dd;
    background-image: linear-gradient(90deg, #5635dd 0%, #e63573 100%);
    position: relative;
    margin-left:5px ;
    margin-top: -25px;
    z-index: 1;
  }

.miami {
  font-size: 170px;
  font-weight: bold;
  margin-top: -180px;
  margin-bottom: 200px;
  background: linear-gradient(90deg, #5635dd, #e63573);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.walker {
    font-size: 170px;
    text-align: end;
    font-weight: bold;
    position: absolute;
    top: 300px;
    left: 170px;
    z-index: 2;
  }

.des {
  color: #666666;
  font-size: 17px;
}
</style>
