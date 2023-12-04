<template>
  <div>
      <div class=" flex flex-col items-center justify-center">
      <div class=" text-5xl text-center  font-bold my-10">
      Our Services
      </div>
      <hr class="  w-1/6  h-2 border-orange-400">
  </div>
   
    <div class="  grid grid-cols-4 gap-5 lg:p-10">
      <div v-for="(item,index) in items" class=" relative  p-5 flex flex-col items-center justify-center space-y-5 hover:shadow-2xl transition-all duration-300" :class="index === 1 ? 'border-orange-500/50 border-4' : 'border-black/20 border '">
        <p class="text-2xl font-serif ">{{ item.title }}</p>
       <div class="flex space-x-2">
         <p class="text-4xl  font-sans font-extralight text-orange-400"> ${{ item.price }}</p><p class="font-bold">/mo</p>
       </div>
       <hr class="w-full      my-10">
        <ul>
          <li v-for="feature in item.features" class="flex  justify-start gap-2 my-4">
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
      'Construction Planning',
      'Cost Containment',
      'General Contracting',
      '1GB Storage',
      'Phone Consultation',
    ]
  },
  {
    title: 'Standard',
    price: 19.99,
    features: [
      'Pre-construction Services',
      'Construction Administration',
      'Virtual Design',
      'Project Management',
    
    ]
  },
  {
    title: 'Business',
    price: 29.99,
    features: [
      'Construction Services',
      'Self-perform',
      'Construction management',
      'Cost Estimation',
  
    ]
  },
  {
    title: 'Professional',
    price: 39.99,
    features: [
      'Design-build',
      'Equipment Installation',
      'Quality Assurance',
      'Green Construction',
 
    ]
  },
]
</script>

<style></style>