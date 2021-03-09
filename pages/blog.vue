<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
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
      title: `Contact | ${this.$siteConfig.siteName}`
    }
  },
  components: {}
}
</script>

<style scoped>
.products-page {
  background-color: yellow;
}
</style>
