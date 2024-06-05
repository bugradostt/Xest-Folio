<template>
  <div class="q-ma-xl">

    <div class="container">

      <div class="title-project">Have you project in mind?</div>
      <div class="des">
        Let’s Make Something
        <br>
Great Together!
      </div>

      <div class="contact">
        CONTACT WITH US
      </div>


      <span class="title-company">
          Xest
          <br>
          Folio
        </span>


        <div class="icon-container">
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-linkedin-in"></i>
        <i class="fab fa-instagram"></i>
        <i class="fab fa-behance"></i>
        <i class="fab fa-dribbble"></i>
    </div>


    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>

.icon-container {
    display: flex;
    gap: 10px;
    justify-content: center;
    align-items: center;
}

.icon-container i {
    font-size: 24px;
    margin: 0 50px;

}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

.title-project {
  text-transform: uppercase;
  background: linear-gradient(90deg, #5635dd, #e63573);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.des {
  font-size: 40px;
  font-weight: bold;
  line-height: 43px;
}


.title-company {
  margin-top: 40px;
  margin-bottom: 40px;
  font-size: 25px;
    background: linear-gradient(180deg, #5635dd, #e63573);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
.contact{
  background-color: #5635dd;
background-image: linear-gradient(180deg, #5635dd 0%, #e63573 100%);
color: white;
margin-top: 30px;
border-radius: 150px;
width: 250px;
height: 250px;
display: flex;
justify-content: center;
align-items: center;
text-align: center;
}
</style>
