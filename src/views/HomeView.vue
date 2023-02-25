<template>
  <div class="bg-dark">
    <section class="slider">
      <Slide />
    </section>
    <section class="discoveres">
      <div class="discover-base"></div>
      <Discover />
    </section>
    <!-- <section class="discover">
    </section> -->
  </div>
</template>

<script>
import Slide from "@/components/home/Slide.vue";
import Discover from "@/components/home/Discover.vue";
export default {
  name: "HomeView",
  components: {
    Slide,
    Discover,
  },
};
</script>
