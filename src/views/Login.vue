<template>
  <div class="login">
    <Header/>
    <LoginBlock/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import LoginBlock from '@/components/LoginBlock.vue'
@Component({
  components: {
    Header,
    LoginBlock,
    Footer
  }
})
export default class Login extends Vue {}
</script>
