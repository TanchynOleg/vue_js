<template>
  <div class="products">
    <Header/>
    <GalleryBlock/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import GalleryBlock from '@/components/GalleryBlock.vue'
@Component({
  components: {
    Header,
    Footer,
    GalleryBlock
  }
})
export default class Products extends Vue {}
</script>
