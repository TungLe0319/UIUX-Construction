<template>
  <div>
    <div class="text-center my-5">
      Pricing
    </div>
    <hr class="w-full h-2 border-orange-400">
    <div class="  grid grid-cols-4 gap-4 lg:p-10">
      <div v-for="(item,index) in items" class=" relative  p-5 flex flex-col items-center justify-center space-y-5 hover:shadow-2xl transition-all duration-300" :class="index === 1 ? 'border-orange-500/50 border-4' : 'border-black/20 border '">
        <p class="text-2xl font-serif ">{{ item.title }}</p>
       <div class="flex space-x-2">
         <p class="text-2xl  text-orange-400"> ${{ item.price }}</p><p class="font-bold">/mo</p>
       </div>
        <ul>
          <li v-for="feature in item.features" class="flex  justify-start gap-2 my-1">
            <Icon name="mdi:check" size="20px" class="text-orange-400" />
       <p>     {{ feature }}</p>
          </li>
        </ul>
        <div class="my-4">
          <v-btn color="orange-lighten-2">Buy Now!</v-btn>
        </div>

        <Icon v-if="index === 1" name="mdi:star" class="text-orange-400 text-7xl absolute -top-12 -left-4" />
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