<template>
  <HeadersComponent />
  <router-view />
  <Footer />
</template>
<script>
import HeadersComponent from "@/components/HeadTemplate.vue";
import Footer from "@/components/Footer.vue";
export default {
  components: {
    HeadersComponent,
    Footer,
  },
};
</script>
