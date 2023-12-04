<template>

    <div class=" flex flex-col items-center justify-center">
        <div class=" text-5xl text-center  font-bold my-10">
        About us
        </div>
        <hr class="  w-1/6  h-2 border-orange-400">
    </div>

   <div class="flex w-full flex-col items-center justify-center  p-10 lg:flex-row ">
      <div class="flex flex-col items-center justify-center lg:w-1/2 lg:pl-10">
          <SectionHeader header="Your Comfort, Our Mission" title="Efficient Heating and Cooling Answers"
            content="Facing issues with inconsistent room temperatures? Our HVAC experts provide tailored solutions to ensure a comfortable environment in every corner of your home. Say goodbye to temperature imbalances and hello to personalized climate control." />
          <div class="mt-3 space-y-8">
            <div class="flex">
              <div class="mx-3 h-fit">
                <Icon name="fluent:person-support-16-filled" class="text-orange-400 text-5xl" />
              </div>
              <div class="lg:w-3/4">
                <div>
                  <h1 class=" text-xl font-bold lg:text-2xl">
                    Responsive Assistance
                  </h1>
               <p class="text-sm lg:text-base">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Voluptas nemo corrupti esse, eveniet quos dignissimos,
                      accusantium soluta, commodi quae nihil cum tempora omnis.
                    </p>
                </div>
              </div>
            </div>
            <div class="flex">
              <div class="mx-3 h-fit">
                <Icon name="ph:certificate-duotone"  class="text-orange-400 text-5xl" />
              </div>
              <div class="lg:w-3/4">
                <div>
                  <h1 class=" text-xl font-bold lg:text-2xl">
                    Proven Quality
                  </h1>
                  <p class="text-sm lg:text-base">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Voluptas nemo corrupti esse, eveniet quos dignissimos,
                    accusantium soluta, commodi quae nihil cum tempora omnis.
                  </p>
                </div>
              </div>
            </div>
              <div class="flex">
                <div class="mx-3 h-fit">
                  <Icon name="fluent:people-team-20-filled"  class="text-orange-400 text-5xl" />
                </div>
                <div class="lg:w-3/4">
                  <div>
                    <h1 class=" text-xl font-bold lg:text-2xl">
                      Proven Quality
                    </h1>
                    <p class="text-sm lg:text-base">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Voluptas nemo corrupti esse, eveniet quos dignissimos,
                      accusantium soluta, commodi quae nihil cum tempora omnis.
                    </p>
                  </div>
                </div>
              </div>
          </div>
        </div>
      <div class="flex w-full items-center justify-center lg:w-1/2 mb-10 lg:mb-0">
        <iframe class="rounded-md shadow-2xl" width="560" height="315"
          src="https://www.youtube.com/embed/NpEaa2P7qZI?si=AYGfNW0zFeyJNnVg" title="YouTube video player" frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen />
      </div>
    
    </div>
</template>

<script lang="ts" setup>
import SectionHeader from '../Globals/SectionHeader.vue';


</script>

<style>

</style>