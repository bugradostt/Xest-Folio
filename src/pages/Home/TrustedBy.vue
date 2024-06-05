<template>
  <div class="q-ma-xl">

    <div class="container">

      <div class="title-trusted">Trusted By</div>


      <div class="image-container">
        <img src="public/img/logo1.png" style="max-width: 150px" />
        <img src="public/img/logo2.png" style="max-width: 150px" />
        <img src="public/img/logo3.png" style="max-width: 150px" />
        <img src="public/img/logo4.png" style="max-width: 150px" />
        <img src="public/img/logo5.png" style="max-width: 150px" />
    </div>




    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>

.image-container {
    display: flex;
    justify-content: center;
    align-items: center;
}

.image-container img {
    margin: 0 50px;
}



.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

.title-trusted {
color: #12141DCC;
opacity: 0.8;
margin: 80px 0 40px 0;
font-weight: bold;
}




</style>
