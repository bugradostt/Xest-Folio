<template>
  <div class="q-ma-xl">



    <div class="container">
  <div>
    <div>Portfolio</div>
    <div>Some Of Our Best Works </div>
  </div>
  <div>
    <div>Load More</div>
  </div>
</div>


    <div class="row">

      <div class="col-4">
        <Card></Card>
      </div>

      <div class="col-4">
        <Card></Card>
      </div>

      <div class="col-4">
        <Card></Card>
      </div>

      <div class="col-4">
        <Card></Card>
      </div>

      <div class="col-4">
        <Card></Card>
      </div>

      <div class="col-4">
        <Card></Card>
      </div>

    </div>
  </div>
</template>

<script setup>
import Card from 'src/components/Card.vue'

</script>

<style scoped>

.container {
    display: flex;
    justify-content: space-between;
  }
</style>

