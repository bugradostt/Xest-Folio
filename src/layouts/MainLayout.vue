<template>
  <q-layout view="lHh Lpr lFf">

    <q-toolbar class="bg-white text-black  ">
      <q-btn flat label="Xest Folio" />
      <q-space />


      <q-tabs v-model="tab" shrink>

        <q-tab name="about" label="About" />
        <q-tab name="service" label="Service" />
        <q-tab name="blogs" label="Blogs" />
        <q-tab name="faq" label="FAQ" />
        <q-tab name="contactMe" label="Contact Me" />

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
</style>
