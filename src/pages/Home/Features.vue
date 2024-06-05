<template>
  <div class="q-ma-xl">

    <div class="container">

      <div>
        <label class="title-features">FEATURES</label>

        <div class="des">
          Giving Your Business
          <br>
          Some Great Ideas

        </div>


        <br>
        <label class="des2">
          Every designer needs the right tools to do the perfect job.
          <br>
          Thankfully, we can do that. I design products that are more
          <br>
          than pretty. I make them shippable and usable.
        </label>
        <br>

        <div>

          <div class="contact-us">
            Contact Us
          </div>

          <div class="contact-us-gradient">

          </div>

        </div>

      </div>

      <div style="display: flex; flex-direction: column; margin-left: 150px;">

        <div style="display: flex; ">

          <div style="margin: 50px 30px 0 0;">
            <img class="img" src="public/img/features1.png" width="271" height="150">

            <div class="title">UX Experience </div>
            <br>
            <label class="des3">I design products that are more
              <br />
              than pretty. I make them usable. </label>
          </div>

          <div>
            <img class="img" src="public/img/features2.png" width="271" height="150">

            <div class="title">UI Design </div>
            <br>
            <label class="des3">I design products that are more
              <br />
              than pretty. I make them usable. </label>
          </div>

        </div>

        <div style="display: flex; ">

          <div style="margin: 50px 30px 0 0;">
            <img class="img" src="public/img/features3.png" width="271" height="150">

            <div class="title">UX Experience </div>
            <br>
            <label class="des3">I design products that are more
              <br />
              than pretty. I make them usable. </label>
          </div>

          <div>
            <img class="img" src="public/img/features4.png" width="271" height="150">

            <div class="title">UI Design </div>
            <br>
            <label class="des3">I design products that are more
              <br />
              than pretty. I make them usable. </label>
          </div>

        </div>


      </div>

    </div>

    <div class="statistic-container">

      <div>
        <div class="statistic-value">12K+</div>
        <div class="statistic-name">Project Complete</div>
      </div>

      <div>
        <div class="statistic-value">7K+</div>
        <div class="statistic-name">Happy Client</div>
      </div>

      <div>
        <div class="statistic-value">10+</div>
        <div class="statistic-name">Years Experience</div>
      </div>

      <div>
        <div class="statistic-value">270+</div>
        <div class="statistic-name">Win Awards</div>
      </div>

    </div>




  </div>
</template>

<script setup>

</script>

<style scoped>

.statistic-container {
    display: flex;
    gap: 10px;
    justify-content: center;
    align-items: center;
}

.statistic-value{

  color: transparent;
  text-align: center;
  font-weight: bold;
  font-size: 70px;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: #991fb5 ;

}
.statistic-name{
  color: black;
  font-weight: 600;
  text-align: center;



}
.statistic-container div {
    margin: 0 50px;

}


.container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin: 50px;

}

.title-features {
  background: linear-gradient(90deg, #5635dd, #e63573);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.des {
  font-size: 30px;
  font-weight: bold;
  line-height: 43px;

}

.des2 {
  color: #AAAAAA;
  margin-top: 20px;
}

.contact-us {
  color: white;
  background-color: black;
  font-size: 12px;
  padding: 10px;
  width: 100px;
  text-align: center;
  position: relative;
  top: 20px;
  z-index: 2;
}

.contact-us-gradient {
  padding: 15px;

  width: 100px;
  height: 100%;
  background-color: #5635dd;
  background-image: linear-gradient(90deg, #5635dd 0%, #e63573 100%);
  position: relative;
  margin-left: 5px;
  margin-top: -5px;
  z-index: 1;
}

.img {
  border-radius: 0 10px 0 10px;
}

.des3 {

  color: #AAAAAA;
}

.title {
  font-weight: bold;
  font-size: 18px;
  margin-top: 5px;

}
</style>
