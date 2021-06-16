<template>
  <div id="app">
    <router-view/>
    <div class="footer">
      <Footer />
    </div>
  </div>
</template>

<script>
import Footer from "@/components/Footer.vue"
export default {
  components: {
    Footer
  }
}
</script>