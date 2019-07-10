<template>
  <div class="home">
    <Header/>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Hello this is Home page with Vue js"/>
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
export default class Home extends Vue {}
</script>
