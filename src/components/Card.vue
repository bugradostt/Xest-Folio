<template>

  <q-card class="card" flat bordered>
    <q-img :src="props.img"  class="img" />
  </q-card>
</template>

<script setup>

import {ref ,defineProps, defineEmits } from 'vue';

const props = defineProps({

  img: {
    type: String,
    default: ""
  },

})


</script>

<style scoped>
.card{
margin: 10px;
}

.img{
  height: 300px;
}
</style>
