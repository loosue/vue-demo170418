<template lang="html">
  <div class="react">
    <my-header></my-header>
    <p>这是React的内容</p>
  </div>
</template>

<script>
import myHeader from './Header/Header'

export default {
  name: 'react',
  data () {
    return {
    }
  },
  components: {
    myHeader
  }
}
</script>

<style lang="css">
</style>
