<template>
  <div id="app">
    <TopBar/>
    <nuxt/>
  </div>
</template>

<script>
import TopBar from '@/components/TopBar'
export default {
  name: 'App',
  components: {
    TopBar
  }
}
</script>
