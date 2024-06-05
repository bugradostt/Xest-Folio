<template>

<q-card class="card">
      <q-card-section class="bg-white text-black " style="box-shadow: none; border: none;">

        <i class=" icon fa-solid fa-quote-left"></i>
        <div class="text-subtitle2 title-value">{{ props.title }}</div>
      </q-card-section>

      <div class="user-star-container">
  <div class="user-info">
    <q-avatar size="30px" text-color="white"  >
      <img :src="props.img" alt="">
    </q-avatar>
    {{ props.user }}
  </div>
  <div class="star">
    <i style="color: #FFB23F;" class="fa-solid fa-star"></i>
    {{ props.star }}
  </div>
</div>

    </q-card>
</template>

<script setup>

import {ref ,defineProps, defineEmits } from 'vue';

const props = defineProps({
  title: {
    type: String,
    default: ""
  },
  user: {
    type: String,
    default: ""
  },
  star: {
    type: String,
    default: ""
  },
  img: {
    type: String,
    default: ""
  },

})


</script>

<style scoped>
.card{
  width: 100%;
  max-width: 300px;
  text-align: left;
}

.icon{
  font-size: 20px;
  background: linear-gradient(180deg, #5635dd, #e63573);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.title-value{
  color: #090D23;
  font-family: Poppins;
  opacity: 0.8;
  text-align: justify;
}

.user-star-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px;
}

.user-info {
  margin-right: 10px;
}

.star {
  padding: 5px;
  border-radius: 5px;
  font-weight: 700;
  font-size: 12px;
}
</style>
