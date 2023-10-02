<template>
  <main>
    <NavigationbarSection />
    <CarouselSection />
    <IntroductionActivities />
    <ActivitiesSection />
  </main>
</template>

<script>
import NavigationbarSection from '@/components/NavigationbarSection.vue'
import CarouselSection from '@/components/CarouselSection.vue'
import IntroductionActivities from '@/components/IntroductionActivities.vue'
import ActivitiesSection from '@/components/ActivitiesSection.vue'
export default {
  components: {
    NavigationbarSection,
    CarouselSection,
    IntroductionActivities,
    ActivitiesSection
  }
}
</script>
