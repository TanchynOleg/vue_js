<template>
  <div class="products">
    <Header/>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
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
export default class Products extends Vue {}
</script>
