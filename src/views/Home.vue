<template>
<span>
    <home-hero></home-hero>
    <home-details></home-details>
    <home-projects></home-projects>
</span>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import HomeHero from '@/components/HomeHero'
import HomeDetails from '@/components/HomeDetails'
import HomeProjects from '@/components/HomeProjects'


export default {
  name: 'home',
  components: {
    HomeHero,
    HomeDetails,
    HomeProjects,
  }
}
</script>
