<template lang="pug">
#app
  nav#nav-bar.no-print.four.item.ui.green.menu
    router-link.item(to="/")
      i.home.icon
      span.fat-only {{ $t('home') }}
    router-link.item(to="/about")
      i.user.icon
      span {{ $t('about_me') }}
    router-link.item(to="/course")
      i.users.icon
      span {{ $t('courses') }}
    router-link.item(to="/map")
      i.map.icon
      span {{ $t('map') }}
  router-view
  footer.bottom
    a(href="https://www.facebook.com/xiaoxiaoplace", target="_blank", rel="noopener noreferrer")
      i.facebook.icon
      | FB: 小小蔬房
    div
      i.map.icon
      | 地址: 台北市萬華區漢口街二段125號
    div
      i.phone.icon
      | 電話: 02-2311-1168


</template>

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
  bottom: 0;
  right: 0;
  margin: 1em;
  text-align: left;
  width: 300px;
}
</style>
