<template lang="html">

  <section id="experience" class="experience">
    <h1>Experience Component</h1>
    <Subcomponent
      title="University of Notre Dame"
      text="Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Vivamus sit amet mauris nec augue molestie laoreet. Phasellus molestie
      tortor a vestibulum tempor. Proin malesuada blandit leo, eget varius eros
      viverra non. Sed porta tristique lorem non pharetra. Suspendisse turpis
      ex, rhoncus in faucibus non, egestas non elit. Aenean eget orci in mauris
      congue gravida id ac enim. Aenean tempus purus sed mi dignissim congue.
      Proin lorem risus, luctus pulvinar tincidunt ut, scelerisque eu dui.
      Donec sodales semper aliquam. Sed mollis ante dignissim, sollicitudin
      orci nec, pretium ex. Proin et lobortis nisl. Curabitur ullamcorper non
      turpis id efficitur. Ut eu lectus volutpat augue pretium maximus."
      image="https://via.placeholder.com/300x300"
      orientation="right"
    />
    <Subcomponent
      title="University of Notre Dame"
      text="Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Vivamus sit amet mauris nec augue molestie laoreet. Phasellus molestie
      tortor a vestibulum tempor. Proin malesuada blandit leo, eget varius eros
      viverra non. Sed porta tristique lorem non pharetra. Suspendisse turpis
      ex, rhoncus in faucibus non, egestas non elit. Aenean eget orci in mauris
      congue gravida id ac enim. Aenean tempus purus sed mi dignissim congue.
      Proin lorem risus, luctus pulvinar tincidunt ut, scelerisque eu dui.
      Donec sodales semper aliquam. Sed mollis ante dignissim, sollicitudin
      orci nec, pretium ex. Proin et lobortis nisl. Curabitur ullamcorper non
      turpis id efficitur. Ut eu lectus volutpat augue pretium maximus."
      image="https://via.placeholder.com/300x300"
      orientation="left"
    />
    <Subcomponent
      title="University of Notre Dame"
      text="Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Vivamus sit amet mauris nec augue molestie laoreet. Phasellus molestie
      tortor a vestibulum tempor. Proin malesuada blandit leo, eget varius eros
      viverra non. Sed porta tristique lorem non pharetra. Suspendisse turpis
      ex, rhoncus in faucibus non, egestas non elit. Aenean eget orci in mauris
      congue gravida id ac enim. Aenean tempus purus sed mi dignissim congue.
      Proin lorem risus, luctus pulvinar tincidunt ut, scelerisque eu dui.
      Donec sodales semper aliquam. Sed mollis ante dignissim, sollicitudin
      orci nec, pretium ex. Proin et lobortis nisl. Curabitur ullamcorper non
      turpis id efficitur. Ut eu lectus volutpat augue pretium maximus."
      image="https://via.placeholder.com/300x300"
      orientation="right"
    />
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import Subcomponent from '@/components/Subcomponent.vue';

@Component({
  components: {
    Subcomponent,
  },
})
export default class Experience extends Vue {
}
</script>

<style scoped lang="scss">
  .experience {

  }
</style>
