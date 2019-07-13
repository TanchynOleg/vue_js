<template>
  <div class="home">
    <Header/>
    <TextBlock/>
    <HelloWorld msg="Hello this is Home page with Vue js"/>
    <DateBlock/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import HelloWorld from '@/components/HelloWorld.vue'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import ContactBlock from '@/components/ContactBlock.vue'
import DateBlock from '@/components/DateBlock.vue'
import TeamBlock from '@/components/TeamBlock.vue'
import TextBlock from '@/components/TextBlock.vue'

@Component({
  components: {
    TeamBlock,
    TextBlock,
    HelloWorld,
    Header,
    Footer,
    ContactBlock,
    DateBlock
  }
})
export default class Home extends Vue {}
</script>
