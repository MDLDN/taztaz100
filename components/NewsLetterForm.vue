<template>
  <div>
    <form
      target="_blank"
      method="post"
      :action="formAction"
      @submit="$emit('submit', email)"
    >
      <div class="field has-addons is-fullwidth tel">
        <p class="control">
          <a href="tel:078-402-57052">078 402 57052 </a>
        </p>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: ''
    }
  },
  computed: {
    formAction() {
      if (this.$siteConfig.newsletter.mailchimp.on) {
        return this.$siteConfig.newsletter.mailchimp.formAction
      }
      return this.$siteConfig.newsletter.custom.formAction
    }
  }
}
</script>
