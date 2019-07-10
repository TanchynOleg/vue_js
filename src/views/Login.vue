<template>
  <div class="about">
    <Header/>
    <Login/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import HelloWorld from '@/components/HelloWorld.vue'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import Login from '@/components/Login.vue'
import ContactBlock from '@/components/ContactBlock.vue'
@Component({
  components: {
    HelloWorld,
    Header,
    Footer,
    Login,
    ContactBlock
  }
})
export default class About extends Vue {}
</script>