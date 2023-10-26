<template>
  <main>
    <CarouselSection />
    <IntroductionActivities />
    <ActivitiesSection />
    <MapSection />
  </main>
</template>

<script>
import CarouselSection from '@/components/CarouselSection.vue'
import IntroductionActivities from '@/components/IntroductionActivities.vue'
import ActivitiesSection from '@/components/ActivitiesSection.vue'
import MapSection from '@/components/MapSection.vue'
export default {
  components: {
    CarouselSection,
    IntroductionActivities,
    ActivitiesSection,
    MapSection
  }
}
</script>
