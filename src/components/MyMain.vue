<template>
  <div>
    <KeyFeatures/>
    <SectionDue/>
    <SectionTre/>
    <SectionQuattro/>
    <SectionCinque/>
  </div>
</template>

<script>
import KeyFeatures from '@/components/KeyFeatures.vue'
import SectionDue from '@/components/SectionDue.vue'
import SectionTre from '@/components/SectionTre.vue'
import SectionQuattro from '@/components/SectionQuattro.vue'
import SectionCinque from '@/components/SectionCinque.vue'

export default {
  name: 'MyMain',
  components:{
    KeyFeatures,
    SectionDue,
    SectionTre,
    SectionQuattro,
    SectionCinque
  }

}
</script>


<style scoped lang="scss">
</style>