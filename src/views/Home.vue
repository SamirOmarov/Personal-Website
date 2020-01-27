<template>
<span>
    <home-hero></home-hero>
    <home-details></home-details>
    <home-projects></home-projects>
    <home-tech-stack></home-tech-stack>
    <home-contact></home-contact>
</span>
</template>

<script>
// @ is an alias to /src

import HomeHero from '@/components/HomeHero'
import HomeDetails from '@/components/HomeDetails'
import HomeProjects from '@/components/HomeProjects'
import HomeTechStack from '@/components/HomeTechStack'
import HomeContact from '@/components/HomeContact'

export default {
  name: 'home',
  components: {
    HomeHero,
    HomeDetails,
    HomeProjects,
    HomeTechStack,
    HomeContact
  }
}
</script>