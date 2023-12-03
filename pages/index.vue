<script lang="ts" setup>
import CallToAction from '~/components/Globals/CallToAction.vue';
import About from '~/components/Index/About.vue';

import BusinessHours from '~/components/Index/BusinessHours.vue';
import Hero from '~/components/Index/Hero.vue';
import LandingPhotoGallery from '~/components/Index/LandingPhotoGallery.vue';
import Testimonials from '~/components/Index/Testimonials.vue';
</script>

<template>
  <div class="flex flex-col  ">
    <Hero />
    <About/>
    <CallToAction />
    <Projects/>
    <BusinessHours />
    <LandingPhotoGallery />
    <Testimonials />
  </div>
</template>


<style scoped></style>
