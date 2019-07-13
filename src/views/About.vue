<template>
  <div class="about">
    <Header/>
    <TeamBlock/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import ContactBlock from '@/components/ContactBlock.vue'
import TeamBlock from '@/components/TeamBlock.vue'
@Component({
  components: {
    TeamBlock,
    Header,
    Footer,
    ContactBlock
  }
})
export default class About extends Vue {}
</script>
