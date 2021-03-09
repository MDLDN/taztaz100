<template>
  <div id="services-page" class="page-wrapper services-page content-page">
    <main-section width="contained" theme="one-column">
      <template v-slot:default>
        <div class="content">
          <h5 class="button red is-small">
            Services
          </h5>
        </div>
      </template>
    </main-section>
  </div>
</template>
<script>
import { setPageData } from '../helper'
export default {
  head() {
    return {
      title: `Services | ${this.$siteConfig.siteName}`
    }
  },
  data() {
    return { stories: [], docs: [] }
  },
  fetch({ store, params }) {
    setPageData(store, { slug: 'products' })
  },
  // eslint-disable-next-line no-dupe-keys
  async fetch() {
    try {
      const query = await this.$prismic.api.query(
        this.$prismic.predicates.at('document.type', 'product'),
        { orderings: '[my.product.position]' }
      )
      this.docs = query.results
    } catch (e) {
      console.log(e)
    }
  },
  fetchDelay: 500
}
</script>
<style scoped>
.button {
  background-color: black;
  color: yellow;
}
</style>
