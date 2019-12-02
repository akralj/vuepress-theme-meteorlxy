<template>
  <div id="vuepress-theme-meteorlxy" :class="layoutClass">
    <TheHeader />

    <TheMain />

    <TheFooter />
  </div>
</template>

<script>
import TheHeader from '../components/TheHeader.vue'
import TheMain from '../components/TheMain.vue'
import TheFooter from '../components/TheFooter.vue'

export default {
  name: 'ThemeMeteorlxy',

  components: {
    TheHeader,
    TheMain,
    TheFooter,
  },

  computed: {
    layoutClass () {
      return "layout-" + this.$frontmatter.layout;
    }
  }

}
</script>

<style lang="stylus" src="../styles/index.styl" />
