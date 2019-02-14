<template lang="html">

  <section class="stars">
    <span v-for="n in numberChecked" class="fa fa-star checked"></span>
    <span v-for="n in (5 - numberChecked)" class="fa fa-star"></span>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Stars extends Vue {
  @Prop() private numberChecked!: number;
}
</script>

<style scoped lang="scss">
  .stars {
    font-size: 2em;
    min-width: 180px;
  }
  .checked {
    color: orange;
  }
</style>
