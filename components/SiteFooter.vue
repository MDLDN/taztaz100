<template>
  <footer class="site-footer">
    <section class="hero is-small">
      <div class="hero-body">
        <div class="container">
          <div class="columns">
            <div class="column">
              <h3>
                <div class="notification">
                  <p>
                    Opening Hours
                  </p>
                  <p>24 Hours!</p>
                  <p>On Demand!</p>
                </div>
              </h3>
            </div>
            <div class="column">
              <figure>
                <p class="logoname">
                  The TazTaz
                </p>
              </figure>
              <div>
                <p>71-75 Shelton Street</p>
                <p>Covent Garden</p>
                <p>London</p>
                <p>WC2H 9JQ</p>
                <p>England</p>
                <a href="tel:078-402-57052">078 402 57052 </a>
                <p>
                  <a href="mailto:info@thetaztaz.com">
                    info@thetaztaz.com
                  </a>
                </p>
                <p class="sociallogo">
                  @taztaz_official
                </p>
              </div>
            </div>
            <div class="column">
              <div class="notification has-background-black">
                <div class="container center">
                  <news-letter-form />
                </div>
                <div class="container socialicons">
                  <a href="https://twitter.com/">
                    <b-icon
                      icon="twitter"
                      custom-size="fa-lg"
                      type="primary"
                    ></b-icon>
                  </a>
                  <a href="https://instagram.com/">
                    <b-icon
                      icon="instagram"
                      custom-size="fa-lg"
                      type="primary"
                    ></b-icon>
                  </a>
                  <a href="https://www.youtube.com/">
                    <b-icon icon="youtube" custom-size="fa-lg"></b-icon>
                  </a>
                  <a href="https://www.facebook.com//">
                    <b-icon
                      icon="facebook"
                      size="is-medium"
                      custom-size="fa-lg"
                      type="primary"
                    ></b-icon>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="has-background footersig bottom">
      <div class="container is-fluid">
        <div class="columns">
          <div class="column">
            <small>
              {{ $siteConfig.siteName }} LTD Company Number 11049817 England and
              Wales &copy; {{ new Date().getFullYear() }} - All Rights Reserved
              <br />
              <figure>
                <p>The TazTaz</p>
              </figure>
            </small>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import NewsLetterForm from '~/components/NewsLetterForm'
export default {
  name: 'SiteFooter',
  components: {
    NewsLetterForm
  }
}
</script>

<style scoped>
footer {
  background: yellow;
  transition: 0.5s ease all;
  text-align: center;
  color: black;
}
.footersig {
  background-color: black;
  color: yellow;
}
.ftflag {
  width: 35px;
  height: 35px;
  text-align: center;
}
.logo {
  max-width: 150px;
  max-height: 150px;
}
.center {
  display: flex;
  justify-content: center;
  align-items: center;
}
.notification {
  background: black;
  color: yellow;
}
.divider {
  display: block;
  height: 1px;
  border: 0;
  border-top: 1px solid #ccc;
  margin: 1em 0;
  padding: 0;
}
.left {
  text-align: left;
}
.ftlinks {
  font: 1em sans-serif;
  font-kerning: normal;
  font-weight: bold;
}
.socialicons {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
h3 a {
  color: white;
}
.logoname {
  font-family: eagle;
  color: black;
  font-weight: bold;
  font-size: x-large;
  font-variant-caps: all-small-caps;
  line-height: 50px;
}
.sociallogo {
  font-family: eagle;
  font-weight: bold;
}
</style>
