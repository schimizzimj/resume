<template>
  <div class="header">
    <img alt="Profile picture of Marcus at Madrid Royal Palace" src="../assets/madrid-alpha-window.png">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Header extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a {
  color: #42b983;
}
.header {
  position: relative;
  margin-bottom: 30px;
}
h1 {
  position: absolute;
  top: 40%;
  left: 15%;
  font-size: 4em;
  transition: font-size 425ms ease;
  // animation: pulse 10s infinite;
}

@keyframes pulse {
  0% {
    font-size: 4em;
  }
  50% {
    font-size: 4.3em;
  }
  100% {
    font-size: 4em;
  }
}

</style>
