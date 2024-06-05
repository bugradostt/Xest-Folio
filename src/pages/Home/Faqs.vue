<template>
  <div class="body text-white" >

    <div class="container">
  <div class="left">
    <q-expansion-item v-model="business" class="expansion" label="How can we help your business?" >
      <q-card class="bg-dark">
        <q-card-section>
          {{ lorem }}
        </q-card-section>
      </q-card>
    </q-expansion-item>

    <q-expansion-item v-model="bisnext" class="expansion" label="What are the advantages of Bisnext" >
      <q-card class="bg-dark">
        <q-card-section>
          {{ lorem }}
        </q-card-section>
      </q-card>
    </q-expansion-item>

    <q-expansion-item v-model="office" class="expansion" label="Let’s find an office near you?" >
      <q-card class="bg-dark">
        <q-card-section>
          {{ lorem }}
        </q-card-section>
      </q-card>
    </q-expansion-item>

    <q-expansion-item v-model="consultancy" class="expansion" label="How IT consultancy experts work?" >
      <q-card class="bg-dark">
        <q-card-section>
          {{ lorem }}
        </q-card-section>
      </q-card>
    </q-expansion-item>
  </div>

  <div class="right">


    <label class="faqs">
      FAQS
    </label>
    <br>
    <label class="title">
  Be Kind to Your Mind Question & Answer
</label>
    <br>
    <label class="text-grey">All Your Qustions are in A document, in question and answer format, that introduces newcomers to a topic or answers common questions.</label>
  </div>
</div>



  </div>
</template>

<script setup>
import { ref } from 'vue'

var business= ref(false)
var bisnext= ref(false)
var office= ref(false)
var consultancy= ref(false)

var lorem = " Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem, eius reprehenderit eos corrupti commodi magni quaerat ex numquam, dolorum officiis modi facere maiores architecto suscipit iste eveniet doloribus ullam aliquid."

</script>

<style  >

.faqs{
  background: linear-gradient(90deg, #5635dd, #e63573);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.title{
  font-size: 40px;
  line-height: 1;
  max-width: 80%;
}

.body{
  background-color: #181818;
  padding: 50px;
}

.expansion{
  background-color: #222222;
  margin: 10px;
}

.container {
  display: flex;
}

.left {
  flex: 1;
}

.right {
  flex: 1;
  padding: 50px;
}

</style>

