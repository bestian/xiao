<template lang="pug">
#app
  nav#nav-bar.no-print.four.item.ui.green.menu
    router-link.item(to="/")
      i.home.icon
      span.fat-only {{ $t('home') }}
    router-link.item(to="/about")
      i.user.icon
      span.fat-only {{ $t('about_me') }}
    router-link.item(to="/course")
      i.users.icon
      span.fat-only {{ $t('courses') }}
    router-link.item(to="/map")
      i.map.icon
      span.fat-only {{ $t('map') }}
  router-view
  footer.bottom
    a(href="https://www.facebook.com/xiaoxiaoplace", target="_blank", rel="noopener noreferrer")
      i.facebook.icon
      | FB: 小小蔬房
    div
      router-link(to="/map")
        i.map.icon
        | 地址: 台北市萬華區漢口街二段125號
    div
      a(href="tel:0223111168")
        i.phone.icon
        | 電話: 02-2311-1168
</template>

<script type="text/javascript">
import { defineComponent } from 'vue'
import { useHead } from 'unhead'


export default defineComponent({
  name: 'App',
  mounted () {
    useHead({
      title: this.$t('title') + this.$t('xiao')
    })    
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #62f983 !important;
}

.ui.green.menu {
  background-color: #2c7e50;
}

footer.bottom {
  position: fixed;
  background-color: white;
  z-index: 9;
  bottom: 0;
  right: 0;
  padding: 1em;
  text-align: left;
  width: 300px;
}


@media screen and (min-width: 661px) {
  .thin-only {
    display: none !important;
  }
}

@media screen and (max-width: 660px) {
  .fat-only {
    display: none !important;
  }
}

.print-only {
  visibility: hidden;
}

@media print {
  .no-print {
    visibility: hidden;
  }

  .print-only {
    visibility: visible;
  }
}
</style>
