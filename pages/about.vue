<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <main-section width="contained" theme="one-column">
      <template v-slot:default>
        <h5 class="button is-small">
          About
        </h5>
        <br />
        <br />
        <div class="content notification">
          <h3 class="center">
            THE TAZTAZ LTD
          </h3>
          <p class="center">
            <strong>
              Company Number 13096443 England and Wales
            </strong>
          </p>
          <p>
            Nature of business (SIC) <br />
            49390 - Other passenger land transport
            <br />
            49420 - Removal services<br />
          </p>
          <p class="center">
            THE TAZTAZ LTD, is a Private limited Company Incorporated on 22
            December 2020 !
          </p>
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
      </template>
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  'carousel-demo': {
    slidesToScroll: 1,
    slidesToShow: 4
  },
  components: {}
}
</script>

><style scoped>
.button {
  background-color: black;
  color: yellow;
}
.content {
  background-color: black;
  color: yellow;
}
h3 {
  color: yellow;
}
</style>
