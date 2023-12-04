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
    <div id="hero-section">
      <Hero />
    </div>


   
    <div id="about-section">
      <About />
    </div>
    <div id="callToAction-section">
      <CallToAction />
    </div>
    <div id="features-section">
      <Features />
    </div>
    <div id="pricing-section">
      <Pricing />
    </div>
    <div id="projects-section">
      <Projects />
    </div>
    <div id="testimonials-section">
      <Reviews/>
    </div>
    <div id="contact-section">
      <ContactForm />
    </div>
  </div>
</template>


<style scoped></style>
