<template>
  <div class="q-ma-xl">

    <div class="container">

      <div class="title-testimonials">Testimonials</div>
      <div class="des">
        What our customer say
      </div>


    </div>

    <div class="carousel-container">
      <button @click="prev" class="carousel-button prev">‹</button>
      <div class="carousel-wrapper">
        <div v-for="(i, index) in visibleComments" :key="index"
          :class="['carousel-item', { 'is-active': index === 1 }]">
          <div class="comment-content">

            <CardTestimonials :title="i"></CardTestimonials>
          </div>
        </div>
      </div>
      <button @click="next" class="carousel-button next">›</button>
    </div>


  </div>


</template>

<script setup>
import { ref, computed } from 'vue'
import CardTestimonials from 'src/components/CardTestimonials.vue'




var slide = ref('style')



const comments = ref([
  'Yorum 1',
  'Yorum 2',
  'Yorum 3',
  'Yorum 4',
  'Yorum 5',
  'Yorum 6',
  'Yorum 7'
]);

const activeIndex = ref(2);

const prev = () => {
  activeIndex.value = (activeIndex.value - 1 + comments.value.length) % comments.value.length;
};

const next = () => {
  activeIndex.value = (activeIndex.value + 1) % comments.value.length;
};

const visibleComments = computed(() => {
  const prevIndex = (activeIndex.value - 1 + comments.value.length) % comments.value.length;
  const nextIndex = (activeIndex.value + 1) % comments.value.length;
  return [
    comments.value[prevIndex],
    comments.value[activeIndex.value],
    comments.value[nextIndex]
  ];
});



</script>


<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

.title-testimonials {
  background: linear-gradient(90deg, #5635dd, #e63573);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.des {
  font-size: 40px;
  font-weight: bold;
  line-height: 43px;
}



.carousel-container {
  padding: 50px;
  position: relative;
  width: 80%;
  margin: auto;
  overflow: hidden;
  display: flex;
  align-items: center;
}

.carousel-wrapper {
  display: flex;
  justify-content: center;
  width: 100%;
  transition: transform 0.5s ease;
}

.carousel-item {
  flex: 1;
  margin: 0 1%;
  opacity: 0.5;
  transition: transform 0.5s ease, opacity 0.5s ease;
  text-align: center;
}

.carousel-item.is-active {
  transform: scale(1.2);
  opacity: 1;
}

.carousel-button {
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  border: none;
  padding: 1em;
  cursor: pointer;
  z-index: 1;
}

.carousel-button.prev {
  margin-right: -1.5em;
}

.carousel-button.next {
  margin-left: -1.5em;
}
</style>
