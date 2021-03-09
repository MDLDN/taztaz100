<template>
  <div class="logo-wrapper">
    <div class="logo-inner">
      <p>The TazTaz</p>
    </div>
  </div>
</template>
<script>
export default {
  name: 'SiteLogo',
  data() {
    return {
      frames: 5,
      currentFrame: 1,
      blinking: true
    }
  },
  mounted() {
    setInterval(() => {
      const rand = Math.ceil(Math.random() * 10)
      this.blinking = rand % 2
    }, 1000)
  }
}
</script>
<style lang="scss">
@keyframes logoBlink {
  100% {
    transform: translateY(-360px);
  }
}
.logo-wrapper {
  position: relative;
  height: 50px;
  overflow: hidden;
  width: 200px;
  .logo-inner {
    position: absolute;
    height: 500px;
    p {
      font-family: eagle;
      color: black;
      font-weight: bold;
      font-size: x-large;
      font-variant-caps: all-small-caps;
      line-height: 50px;
    }
  }
}
</style>
