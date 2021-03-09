<template>
  <div id="blog-page" class="page-wrapper blog-page content-page">
    <main-section theme="one-column">
      <template v-slot:default>
        <posts-grid />
      </template>
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `Blog | ${this.$siteConfig.siteName}`
    }
  },
  components: {}
}
</script>

<style scoped>
.blog-page {
  background-color: yellow;
}
</style>
