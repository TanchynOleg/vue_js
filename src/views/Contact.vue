<template>
  <div class="contact">
    <Header/>
    <ContactBlock/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import ContactBlock from '@/components/ContactBlock.vue'
@Component({
  components: {
    Header,
    Footer,
    ContactBlock
  }
})
export default class Contact extends Vue {}
</script>
