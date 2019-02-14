<template lang="html">

  <section id="footer" class="footer">
    <h1>Well that's me.</h1>
    <h1>Let me know if you want to <a href="mailto:mschimiz@nd.edu">connect</a>.</h1>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Footer extends Vue {

}
</script>

<style scoped lang="scss">
  .footer {
    padding-top: 20px;
  }
  h1 {
    font-size: 3em;
  }
  a {
    text-decoration: none;
  }
  a:hover {
    color: green;
  }
</style>
