<template lang="html">

  <section class="subcomponent">
    <template v-if="orientation === 'left'">
      <div class="third float">
        <h2>{{title}}</h2>
      </div>
      <div class="third float">
        <p>{{text}}</p>
      </div>
      <div class="third float">
        <img :src="image">
      </div>
    </template>
    <template v-else-if="orientation === 'right'">
      <div class="third float">
        <img :src="image">
      </div>
      <div class="third float">
        <p>{{text}}</p>
      </div>
      <div class="third float">
        <h2>{{title}}</h2>
      </div>
    </template>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Sub extends Vue {
  @Prop() private title!: string;
  @Prop() private text!: string;
  @Prop() private image!: string;
  @Prop() private orientation!: string;
}
</script>

<style scoped lang="scss">
  $height: 300px;
  .subcomponent {
    height: $height;
  }
  .float {
    float: left;
  }
  .third {
    width: calc(100%/3);
    height: $height;
  }
  h2 {
    font-weight: bold;
    font-size: 48px;
  }
</style>
