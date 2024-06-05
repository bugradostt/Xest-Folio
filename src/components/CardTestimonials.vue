<template>

<q-card class="card">
      <q-card-section class="bg-white text-black " style="box-shadow: none; border: none;">
        <div class="text-subtitle2">{{ props.title }}</div>
      </q-card-section>

      <q-card-actions align="around">
        <q-btn flat>Action 1</q-btn>
        <q-btn flat>Action 2</q-btn>
      </q-card-actions>
    </q-card>
</template>

<script setup>

import {ref ,defineProps, defineEmits } from 'vue';

const props = defineProps({
  title: {
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
  max-width: 300px}

</style>
