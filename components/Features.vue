<template>
  <div>
    <div class="text-center my-5">
      Pricing
    </div>
    <hr class="w-full h-2 border-orange-400">
    <div class=" flex gap-5 lg:p-10">
      <div v-for="item in items" class="border border-black/20 p-5">
        <span> {{ item.title }}</span>
        <span> {{ item.icon }}</span>
       <span> {{ item.content }} </span>
        <div class="my-4">
          <v-btn>Buy Now!</v-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
//generate a list of items that has title icon and content 12 of them  and use random MDI icons 

const items = [
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi-coffee',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },

]

</script>

<style></style>