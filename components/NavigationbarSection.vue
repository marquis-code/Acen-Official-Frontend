<template>
  <header class="text-gray-400 bg-gray-900 body-font">
    <div class="container mx-auto flex flex-wrap px-5 py-3 flex-col md:flex-row items-center">
      <a class="flex title-font font-medium items-center text-white">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          class="w-10 h-10 text-white p-2 bg-indigo-500 rounded-full"
          viewBox="0 0 24 24"
        >
          <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" />
        </svg>
        <span class="ml-3 text-xl">ACEN</span>
      </a>
      <nav class="md:mr-auto md:ml-4 md:py-1 md:pl-4 md:border-l md:border-gray-700 flex flex-wrap items-center text-base justify-center">
        <nuxt-link v-for="{name, url} in navItems" :key="name" class="mr-5 hover:text-white" :to="url">
          {{ name }}
        </nuxt-link>
      </nav>
      <button class="flex items-center gap-x-3 bg-gray-800 border-0 py-2.5 px-3 focus:outline-none hover:bg-gray-700 rounded text-sm">
        Become a member
        <span class="relative flex h-2 w-2">
          <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75" />
          <span class="relative inline-flex rounded-full h-2 w-2 bg-sky-500" />
        </span>
      </button>
    </div>
  </header>
</template>

<script>
export default {
  data () {
    return {
      navItems: [
        {
          name: 'News',
          url: '/news'
        },
        {
          name: 'Events',
          url: '/events'
        },
        {
          name: 'Publications',
          url: '/publications'
        },
        {
          name: 'Grants & Awards',
          url: '/grants-and-wards'
        },
        {
          name: 'Membership',
          url: '/membership'
        }
      ]
    }
  }
}
</script>

<style>

</style>
