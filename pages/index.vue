<template>
  <div id="home-page" class="page-wrapper home-page">
    <site-hero :title="title" :subtitle="subtitle" :image="featureImage">
      <button
        v-if="$siteConfig.newsletter.on"
        class="button is-black"
        @click="$eventBus.$emit('modal-triggered', 'newsletter-modal')"
      >
        <p class="call">
          Call
        </p>
      </button>
    </site-hero>
    <section class="hero is-medium is-link">
      <div class="hero-body">
        <p class="title center">
          Servicing London and Environs!
        </p>
        <p class="subtitle center">
          AT YOUR CONVINIENCE
        </p>
        <div class="notification">
          <p>
            Hello Everyone, We are hoping all of you are doing great in this
            unprecedented period. First of all we would like to make a promise
            to Our Customers that we will do our best to solve any kind of
            request in the best possible way. We are a proactive and productive
            business that only aim to fulfil Our Customer’s demands. We will
            always try to answer every call or message as soon as possible. If
            we do not answer, please leave a voice or written message. And we
            will get back to you as fast as we can. Because communication is the
            key role to success for every businesses. We will act with integrity
            and transparency at all times. Our portfolio strength creates
            product quality in all the segments of Customer’s budget bringing
            out uniformity in our operations to build up and be reliable at all
            times. We would like to be part of your lives in the most
            professional way possible, by designing a personalised service
            according to your needs and timings. We are the Win-Win Service that
            priorities Our Customer’s necessities amongst everything else and
            best overall customer satisfaction. A friendly approach that leaves
            its mark forever. A remarkable and unique Service. Kind regards The
            Director
          </p>
        </div>
      </div>
    </section>
    <main-section theme="one-column">
      <template v-slot:sidebar>
        Nothing here
      </template>
    </main-section>
    <news-letter-form-modal />
  </div>
</template>

<script>
import { mapState } from 'vuex'
import { setPageData } from '../helper'
import NewsLetterFormModal from '~/components/NewsLetterFormModal'

export default {
  name: 'HomePage',
  head() {
    return {
      title: `Home | ${this.$siteConfig.siteName}`
    }
  },
  components: {
    NewsLetterFormModal
  },
  computed: {
    ...mapState(['title', 'subtitle', 'featureImage'])
  },
  fetch({ store, params }) {
    setPageData(store, { slug: 'home' })
  }
}
</script>

<style>
.home-page .under-subtitle {
  border-top: none;
}
.home-page {
  background-color: yellow;
}
button {
  background-color: black;
  color: black;
}
.call {
  color: yellow;
}
.center {
  display: flex;
  justify-content: center;
  align-items: center;
}
.notification {
  background-color: black;
  color: yellow;
}
</style>
