<template lang="pug">
div
  TheHeader(@sidenavToggle="displaySidenav = !displaySidenav")
  TheSidenav(:show="displaySidenav" @close="displaySidenav = false")
  nuxt
</template>

<script>
import TheHeader from '@/components/Navigation/TheHeader'
import TheSidenav from '@/components/Navigation/TheSidenav'

export default {
  components: {
    TheHeader,
    TheSidenav
  },
  data () {
    return {
      displaySidenav: false
    }
  }
}
</script>
