<template>
   <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card bg-transparent" flat >
      <q-img
        :src="props.img"
      />



        <q-card-section style="margin: -60px 0 0 40px; background-color: #181818;">
        <div class="text-overline text-grey">  {{ props.overline }}</div>
        <div class="text-h5 q-mt-sm q-mb-xs">{{ props.title }}</div>
        <div class="text-caption text-grey">
          {{ props.des }}
        </div>
      </q-card-section>
      <q-btn flat color="white" label="READ MORE"  style="margin: -60px 0 0 40px; background-color: #181818;">
        <i style="margin-left: 10px;" class="fa-solid fa-arrow-up-right-from-square"></i>
      </q-btn>







    </q-card>
  </div>
</template>

<script setup>
import {ref ,defineProps, defineEmits } from 'vue';

const props = defineProps({
  overline: {
    type: String,
    default: ""
  },

  title: {
    type: String,
    default: ""
  },
  img: {
    type: String,
    default: ""
  },
  des: {
    type: String,
    default: ""
  },
})


var expanded= ref(false)

</script>

<style  scoped>
.my-card{
  width: 100%;
  max-width: 350px}
</style>
