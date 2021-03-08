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
          0784 025 7052
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
