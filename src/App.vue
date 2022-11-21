<template lang="pug">
  #app
    sui-menu#nav-bar.no-print(:widths="7" inverted="")
      sui-menu-item
        router-link(to="/")
          sui-icon(name="home")
          span.fat-only {{ $t('home') }}
      sui-menu-item
        router-link(to="/about")
          sui-icon.fat-only(name="user")
          span {{ $t('about_me') }}
      sui-menu-item
        router-link(to="/comments")
          sui-icon.fat-only(name="comments")
          span.fat-only {{ $t('clients') }}
          span {{ $t('comments') }}
      sui-menu-item
        router-link(to="/course")
          sui-icon.fat-only(name="users")
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
