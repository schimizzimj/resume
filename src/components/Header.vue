<template>
  <div class="header">
    <img alt="Profile picture of Marcus at Madrid Royal Palace" src="../assets/madrid-alpha-window.png">
    <h1 class="not-mobile">Marcus J. Schimizzi</h1>
    <h1 class="if-mobile left-align">Marcus<br />J.<br />Schimizzi</h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Header extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a {
  color: #42b983;
}
.header {
  position: relative;
  margin-bottom: 30px;
  @media screen and (max-width: 600px) {
    img {
      width: 100%;
    }
    h1 {
      top: 10%;
      font-size: 2em;
      color: silver;
    }
  }
}
img {
  width: 100vw;
}
h1 {
  position: absolute;
  top: 40%;
  left: 15%;
  font-size: 4em;
  transition: font-size 425ms ease;
  // animation: pulse 10s infinite;
}

.if-mobile {
  display: none;

  @media screen and (max-width: 600px) {
    display: block;
  }
}

.not-mobile {
  @media screen and (max-width: 600px) {
    display: none;
  }
}

.left-align {
  text-align: left;
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
