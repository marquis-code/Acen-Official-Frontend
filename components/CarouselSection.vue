<template>
  <div>
    <client-only>
      <carousel v-bind="options" class="" :pagination-enabled="false" :autoplay="true">
        <slide v-for="(item, index) in slides" :key="index" class="relative">
          <div class="bg-cover bg-center h-[500px]">
            <!-- <img class="w-full object-cover" :src="require(`~/assets/img/${item.imgUrl}`)" alt=""> -->
            <img :src="require(`~/assets/img/${item.imgUrl}.jpg`)" alt="">
          </div>
          <div class="ltr:sm:text-left rtl:sm:text-right absolute backdrop-brightness-50 w-full h-full inset-0">
            <div
              class="ltr:sm:text-left rtl:sm:text-right space-y-6 flex justify-center items-center flex-col backdrop-brightness-50 w-full h-full inset-0"
            >
              <p class="text-white/90 md:mt-6 md:block text-xs md:text-lg md:leading-relaxed text-center">
                {{ item.description }}
              </p>

              <h2 class="text-xl font-bold text-gray-100 sm:text-3xl md:text-5xl text-center">
                {{ item.title }}
              </h2>
              <div class="mt-4 sm:mt-8 w-full gap-x-6 flex justify-center items-center">
                <button
                  class="inline-block text-sm md:text-base rounded-full bg-indigo-600 w-4/12 md:w-1/12 py-2.5 md:py-2.5  font-medium text-white transition hover:bg-indigo-700 focus:outline-none"
                >
                  Read More
                </button>
                <button
                  class="inline-block text-sm md:text-base rounded-full bg-indigo-600 w-4/12 md:w-1/12 py-2.5 md:py-2.5  font-medium text-white transition hover:bg-indigo-700 focus:outline-none"
                >
                  Contact Us
                </button>
              </div>
            </div>
          </div>
        </slide>
      </carousel>
    </client-only>
    <!-- <ssr-carousel v-model="page">
      <slide v-for="slide in slides" :key="slide.id" :index="1">
        <img :src="require(`~/assets/img/${slide.imgUrl}.jpg`)">
      </slide>
    </ssr-carousel>

    <span class="now">Current Page: {{ page + 1 }}</span>
    <button @click="page--">
      Back
    </button>
    <button @click="page++">
      Next
    </button> -->
  </div>
</template>

<script>
// import SsrCarousel from 'vue-ssr-carousel'
// import ssrCarouselCss from 'vue-ssr-carousel/index.css'
export default {
  components: {
    // SsrCarousel
  },
  data () {
    return {
      options: {
        loop: true,
        perPage: 1,
        autoplay: true,
        // showPagination: false,
        speed: 2000,
        autoplayTimeout: 3000
      },

      page: 1,
      slides: [
        {
          id: 1,
          title: 'BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR',
          description: 'BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR',
          imgUrl: 'background'
        },
        {
          id: 1,
          title: 'BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR',
          description: 'BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR',
          imgUrl: 'background'
        },
        {
          id: 1,
          title: 'BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR',
          description: 'BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR BECOME A YOU AND YOUR HORMONES SOCIAL MEDIA CONTENT CREATOR',
          imgUrl: 'background'
        }
      ]
    }
  }
}
</script>
