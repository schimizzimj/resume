<template lang="html">

  <section id="about-me" class="about-me">
    <h1>Here's little bit about me</h1>
    <Subcomponent
      title="Computer Science"
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
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,w_400/v1504125682/prog_vxcr4o.jpg"
      orientation="left"
    />
    <Subcomponent
      title="Music"
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
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,w_400/v1536386558/pexels-photo-164745_ia7yrf.jpg"
      orientation="right"
    />
    <Subcomponent
      title="Camp Kesem"
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
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,w_400/v1536468998/38151529_1729535687101263_3329993719179902976_o_xrn2gl.jpg"
      orientation="left"
    />
    <Subcomponent
      title="Sports"
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
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_crop,h_500,w_500,x_67,y_154/c_scale,h_300/v1536469801/IMG_0788_vwv9b1.jpg"
      orientation="right"
    />
    <Subcomponent
      title="Travel"
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
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,w_400/v1536386991/IMG_6011_dwppov.jpg"
      orientation="left"
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
export default class AboutMe extends Vue {

}
</script>

<style scoped lang="scss">
  .about-me {

  }
</style>
