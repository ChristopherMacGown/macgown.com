<template>
  <div class="page-wrapper">
    <nuxt />
  </div>
</template>


<script>
export default {
  components: {},
  head() {
    return {
      title: 'MacGown & Associates - Cloud Native leadership for modern tech teams',
    }
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()
      setTimeout(() => this.$nuxt.$loading.finish(), 500)
    })
  },
}
</script>

<style>
</style>
