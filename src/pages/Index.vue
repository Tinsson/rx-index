<template>
  <div class="index-box">
    <IndexHeader></IndexHeader>
    <IndexBanner></IndexBanner>
    <IndexPart></IndexPart>
    <IndexFooter></IndexFooter>
  </div>
</template>

<script>
  import IndexHeader from '../components/IndexHeader'
  import IndexBanner from '../components/IndexBanner'
  import IndexPart from '../components/IndexPart'
  import IndexFooter from '../components/IndexFooter'

  export default {
    name: 'IndexBox',
    data () {
      return {

      }
    },
    components: {
      IndexHeader,
      IndexBanner,
      IndexPart,
      IndexFooter
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
