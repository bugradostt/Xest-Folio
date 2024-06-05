<template>
  <q-layout view="lHh Lpr lFf ">

    <q-toolbar class="bg-white text-black q-pa-lg ">
      <q-btn flat >
        <span class="title-company">
          Xest
          <br>
          Folio
        </span>
      </q-btn>
      <q-space />


      <q-tabs v-model="tab" shrink>

        <q-tab name="about" label="About" />
        <q-tab name="service" label="Service" />
        <q-tab name="blogs" label="Blogs" />
        <q-tab name="faq" label="FAQ" />
        <q-tab name="contactMe"  >
          <div>

              <div class="contact-me">
                Contact Me
              </div>

              <div class="contact-me-gradient">

              </div>

            </div>
        </q-tab>

      </q-tabs>
    </q-toolbar>




    <q-page-container>
      <router-view />
    </q-page-container>


    <q-footer bordered class="bg-white text-grey">
    <div class="footer-content q-pa-md">
      <span class="left-content">© 2023 Ideapeel Inc. All Rights Reserved</span>
      <span class="right-content">Privacy Policy | Terms and Conditions</span>
    </div>
  </q-footer>

  </q-layout>
</template>

<script setup>
import { ref } from 'vue';

</script>

<style scoped>
.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  margin: 10px 0 10px 0;
}

.left-content {
  text-align: left;
  margin-left: 150px;
}

.right-content {
  text-align: right;
  margin-right: 150px;
}


.title-company {
    background: linear-gradient(180deg, #5635dd, #e63573);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

.contact-me {
    color: white;
    background-color: black;
    font-size: 12px;
    padding: 10px;
    position: relative;
    z-index: 2;
  }

  .contact-me-gradient {
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
