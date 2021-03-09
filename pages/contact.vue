<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
    <main-section theme="one-column">
      <template v-slot:default>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Hello!
              </p>
              <p class="subtitle">
                What can I do for you?
              </p>
              <figure class="image is-1by1 ">
                <opti-image
                  :src="require('~/assets/uploads/contact-person.jpg').src"
                  :srcset="
                    require('~/assets/uploads/contact-person.jpg').srcSet
                  "
                />
              </figure>
              <br />
              <div class="content">
                <p>
                  <strong>
                    Tasmir A. Director of Operations
                  </strong>
                </p>
                <p>
                  We will always try to answer every call or message as soon as
                  possible. If we do not answer, please leave a voice or written
                  message. And we will get back to you as fast as we can.
                  Because communication is the key role to success for every
                  businesses. We will act with integrity and transparency at all
                  times.
                </p>
              </div>
            </article>
          </div>
          <div class="tile is-parent is-8">
            <article class="tile is-child box">
              <p class="title center">
                Have your say!
              </p>
              <br />
              <div class="content">
                <p class="center">
                  <strong>
                    For Comments, Suggestions and Complaints
                  </strong>
                </p>
                <p>
                  <br />
                  <strong class="center">contact@thetaztaz.com</strong>
                  <br />
                  <strong class="center">facebook.com/@taztaz_official</strong>
                  <br />
                  <strong class="center">twitter.com/@taztaz_official</strong>
                  <br />
                  Looking forward to hearing from you. <br />
                  Yours Faithfuly, <br />
                  Tasmir A., Director of Operations.
                </p>
              </div>
            </article>
          </div>
        </div>
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
.contact-page {
  background-color: yellow;
  color: yellow;
}
.content,
.tile {
  background-color: black;
  color: yellow;
}
.title,
.subtitle,
p,
strong {
  color: yellow;
}
</style>
