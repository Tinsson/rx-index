<template>
  <div id="app">
    <Index />
  </div>
</template>

<script>
import Index from './pages/index'
import './styles/reset.css'

export default {
  name: 'app',
  components: {
    Index
  }
}
</script>

<style>
  #app{
    width: 100%;
  }
</style>
