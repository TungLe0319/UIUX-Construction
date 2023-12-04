<template>
  <div>
    <div class=" text-5xl text-center my-5">
     Features
    </div>
    <hr class="   h-2 border-orange-400">
    <div class="  grid grid-cols-3 gap-5 lg:p-10">
      <div v-motion-slide-visible-bottom v-for="item in items" class="border border-black/20 p-5 hover:shadow-xl transition-all duration-300">
      <div class="flex gap-2 items-center justify-start">
          <Icon :name="item.icon" size="50px" class="text-orange-400" />
          <span class="text-2xl font-serif "> {{ item.title }}</span>
      </div>
       <p class=" my-5"> {{ item.content }} </p>
        <div class="my-4">
          <v-btn color="orange-lighten-2">Buy Now!</v-btn>
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
    icon: 'mdi:thermometer',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:check',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:thermometer-check',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:cog',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:hand-extended',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:hand-heart',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:loading',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },
  {
    title: 'Lorem Ipsum',
    icon: 'mdi:heart',
    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam accusantium quibusdam quos! Velit, incidunt eius!'
  },

]

</script>

<style></style>