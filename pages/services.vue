<template>
  <div id="services-page" class="page-wrapper services-page content-page">
    <main-section width="contained" theme="one-column">
      <template v-slot:default>
        <div class="content">
          <h5 class="button red is-small">
            Services
          </h5>
        </div>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title center">
                Chuffering
              </p>
              <opti-image
                class="center"
                width="500"
                height="500"
                :src="require('~/assets/uploads/taztaz-chuffer.jpeg').src"
                :srcset="require('~/assets/uploads/taztaz-chuffer.jpeg').srcSet"
              />
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title center">
                Airport Transfers
              </p>
              <figure class="image is-1by1">
                <opti-image
                  class="center"
                  width="500"
                  height="500"
                  :src="
                    require('~/assets/uploads/taztaz-airport-transfers.jpeg')
                      .src
                  "
                  :srcset="
                    require('~/assets/uploads/taztaz-airport-transfers.jpeg')
                      .srcSet
                  "
                />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title center">
                Removals
              </p>
              <figure class="image is-1by1">
                <opti-image
                  class="center"
                  width="500"
                  height="500"
                  :src="require('~/assets/uploads/taztaz-removals.jpeg').src"
                  :srcset="
                    require('~/assets/uploads/taztaz-removals.jpeg').srcSet
                  "
                />
              </figure>
            </article>
          </div>
        </div>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title center">
                Storage
              </p>
              <figure class="image is-1by1">
                <opti-image
                  class="center"
                  width="500"
                  height="500"
                  :src="require('~/assets/uploads/taztaz-storage.jpeg').src"
                  :srcset="
                    require('~/assets/uploads/taztaz-storage.jpeg').srcSet
                  "
                />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title center">
                Furniture
              </p>
              <figure class="image is-1by1">
                <opti-image
                  class="center"
                  width="500"
                  height="500"
                  :src="require('~/assets/uploads/taztaz-furniture.jpeg').src"
                  :srcset="
                    require('~/assets/uploads/taztaz-furniture.jpeg').srcSet
                  "
                />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title center">
                Accountant
              </p>
              <figure class="image is-1by1">
                <opti-image
                  class="center"
                  width="500"
                  height="500"
                  :src="require('~/assets/uploads/taztaz-accountant.jpeg').src"
                  :srcset="
                    require('~/assets/uploads/taztaz-accountant.jpeg').srcSet
                  "
                />
              </figure>
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
      title: `Services | ${this.$siteConfig.siteName}`
    }
  }
}
</script>
<style scoped>
.button {
  background-color: black;
  color: yellow;
}
.tile {
  background-color: yellow;
}
.box {
  background-color: black;
}
.services-page {
  background-color: yellow;
}
.title {
  color: whitesmoke;
  font-weight: 800;
  font-family: eagle;
  font-variant-caps: all-small-caps;
}
</style>
