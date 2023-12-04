<template>
  <div class="p-4 lg:p-10">
    <div class="flex flex-col items-center  justify-center  my-10  ">
      <div class="text-4xl  ">Lorem Ipsum Dolur</div>
      <div class="w-full my-5">
        <IconDivider />
      </div>
      <div class=" text-center text-gray-500 my-8 w-2/3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam
        accusantium quibusdam quos! Velit, incidunt eius!</div>
    </div>
    <div class="grid  md:grid-cols-2 lg:grid-cols-4 gap-6  py-10 ">
      <div v-for="item in items" class="  group transition-all duration-200 hover:scale-[1.02] relative">
        <img :src="item.src" alt="coffee cup icon" class=" shadow-2xl w-full  object-cover  h-96">
        <div
          class="absolute bg-orange-400/50 top-0 w-full h-full flex items-center justify-center text-center  scale-0 group-hover:scale-100 transition-all duration-300">
        <div class="text-2xl text-white w-1/2 ">
            {{ item.title }}
        </div>
        </div>
        <div
          class="absolute bg-transparent border-8 border-white/80  top-0 w-full h-full flex items-center justify-center text-center  scale-0 group-hover:scale-75 transition-all duration-300">
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import IconDivider from './Globals/IconDivider.vue';



const items = [
  {
    src: 'https://images.unsplash.com/photo-1600585154340-be6161a56a0c?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
    title: 'Iced Coffee'
  },
  {
    src: 'https://images.unsplash.com/photo-1605276374104-dee2a0ed3cd6?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
    , title: 'Caramel Mocha Oreo Frappe'
  },
  {
    src: 'https://images.unsplash.com/photo-1600585153490-76fb20a32601?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
    , title: 'Cold Brew'
  }
  ,
  { src: 'https://images.unsplash.com/photo-1600047509358-9dc75507daeb?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Cold Brew Plain' }
  ,
  { src: 'https://images.unsplash.com/photo-1604014238170-4def1e4e6fcf?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Vegan Chocolate Cupcakes' }
  ,
  {
    src: 'https://images.unsplash.com/photo-1628744448840-55bdb2497bd4?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
    , title: 'Croissants'
  }
  ,
  { src: 'https://images.unsplash.com/photo-1600047509782-20d39509f26d?q=80&w=2801&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Bagels' }
  ,
  { src: 'https://images.unsplash.com/photo-1600563438938-a9a27216b4f5?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Avocado Toast' }
  ,
  { src: 'https://images.unsplash.com/photo-1523217582562-09d0def993a6?q=80&w=2960&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Avocado Toast' }
  ,
  { src: 'https://images.unsplash.com/photo-1558969763-1e911dcd91e6?w=800&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NDB8fG1vZGVybiUyMGhvbWV8ZW58MHx8MHx8fDA%3D', title: 'Avocado Toast' }
  ,
  { src: 'https://images.unsplash.com/photo-1494526585095-c41746248156?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Avocado Toast' }
  ,
  { src: 'https://images.unsplash.com/photo-1521574873411-508db8dbe55f?q=80&w=2787&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D', title: 'Avocado Toast' }
  ,

]
</script>

<style scoped>
img {
  width: 100%;

  object-fit: cover;




}


/* Add this to your existing stylesheet */
</style>