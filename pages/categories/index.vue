<template>
  <div id="categories-page" class="page-wrapper categories-page">
    <div class="content">
      <h5 class="button red is-small">
        Products
      </h5>
    </div>
    <main-section theme="one-column">
      <categories-grid />
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `Categories | ${this.$siteConfig.siteName}`
    }
  }
}
</script>
