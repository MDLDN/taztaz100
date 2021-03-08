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
                  <p>Mon - Fri</p>
                  <p>09.00-12.00 & 14.30-16.30</p>
                  <p>Sat & Sun</p>
                  <p>Closed</p>
                </div>
              </h3>
            </div>
            <div class="column">
              <figure>
                <img class="logo" :src="`/Eliza-Logo-BFA02F---.png`" />
              </figure>
              <div>
                <p>7 Gatliff Road</p>
                <p>London</p>
                <p>SW1W 8DF</p>
                <p>United Kingdom</p>
                <p>Tel: 07960 686 509</p>
                <p>Fax: xxx xxxx xxxx</p>
                <p>Email: contact@elizaimportexport.com</p>
              </div>
            </div>
            <div class="column">
              <div class="notification has-background-black">
                <div class="container center">
                  <news-letter-form />
                </div>
                <div class="container socialicons">
                  <b-icon
                    icon="twitter"
                    size="is-medium"
                    custom-size="fa-2x"
                    type="primary"
                  ></b-icon>
                  <b-icon
                    icon="facebook"
                    size="is-medium"
                    custom-size="fa-2x"
                    type="primary"
                  ></b-icon>
                  <b-icon
                    icon="instagram"
                    size="is-medium"
                    custom-size="fa-2x"
                    type="primary"
                  ></b-icon>
                  <b-icon
                    icon="youtube"
                    size="is-medium"
                    custom-size="fa-2x"
                  ></b-icon>
                  <b-icon
                    icon="whatsapp"
                    size="is-medium"
                    custom-size="fa-2x"
                  ></b-icon>
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
              {{ $siteConfig.siteName }} Import Export LTD Company Number
              11049817 England and Wales &copy; {{ new Date().getFullYear() }} -
              All Rights Reserved
              <br />
              <figure>
                <img class="ftflag" :src="`/Eliza-Logo-BFA02F---.png`" />
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
</style>
