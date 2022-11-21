<template lang="pug">
#app
  #nav-bar.no-print.three.item.ui.menu
    router-link.item(to="/")
      i.home.icon
      span.fat-only {{ $t('home') }}
    router-link.item(to="/about")
      i.user.icon
      span {{ $t('about_me') }}
    router-link.item(to="/course")
      i.users.icon
      span {{ $t('courses') }}
  router-view
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
