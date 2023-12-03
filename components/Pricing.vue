<template>
  <div>
    <div class="text-center my-5">
      Pricing
    </div>
    <hr class="w-full h-2 border-orange-400">
    <div class=" flex gap-5 lg:p-10">
      <div v-for="item in items" class="border border-black/20 p-5">
        <span> {{ item.title }}</span>
        <span> {{ item.price }}</span>
        <ul>
          <li v-for="feature in item.features">{{ feature }}</li>
        </ul>
        <div class="my-4">
          <v-btn>Buy Now!</v-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
//generate a list of items that has title, pricing and a list of features 
const items = [
  {
    title: 'Start',
    price: 9.99,
    features: [
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
    ]
  },
  {
    title: 'Standard',
    price: 19.99,
    features: [
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
    ]
  },
  {
    title: 'Business',
    price: 29.99,
    features: [
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
    ]
  },
  {
    title: 'Professional',
    price: 39.99,
    features: [
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
      '1GB Storage',
      '10GB Bandwidth',
      '3 Domains',
    ]
  },
]
</script>

<style></style>