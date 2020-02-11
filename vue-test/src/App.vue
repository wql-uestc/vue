<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
import AddEvent from './components/AddEvent'
import Index from './components/Index'

export default {
  name: 'App',
  components: {
    AddEvent,Index
  }
}
</script>

<style>

</style>
