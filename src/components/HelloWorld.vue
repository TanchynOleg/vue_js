<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
body{
  overflow: hidden;
}

h1 {
  font-family: 'Bowlby One SC', cursive;
  font-size: 4vw;
  width: 100vw;
  margin: 20px 0;
  padding-bottom: 20px;
  text-align: center;
  background: linear-gradient(
                  60deg,
                  hsl(0, 75%, 50%) 10%,
                  hsl(20, 75%, 50%) 10%,
                  hsl(20, 75%, 50%) 25%,
                  hsl(50, 75%, 50%) 25%,
                  hsl(50, 75%, 50%) 40%,
                  hsl(130, 75%, 50%) 40%,
                  hsl(130, 75%, 50%) 55%,
                  hsl(200, 75%, 50%) 55%,
                  hsl(200, 75%, 50%) 70%,
                  hsl(260, 75%, 50%) 70%,
                  hsl(260, 75%, 50%) 85%,
                  hsl(0, 75%, 50%) 85%
  );
  text-shadow: 0.5px -0.6vw #fff4;
  color: #fff;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: 10s BeProud linear infinite,
  3s Always ease alternate infinite;
}

@keyframes BeProud {
  100% { background-position: 100vw 0px; }
}

@keyframes Always {
  100% { transform: scale(1.1);}
}
</style>
