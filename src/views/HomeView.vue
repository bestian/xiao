<template>
  <div class="home">
    <HelloI18n/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloI18n from '@/components/HelloI18n.vue'

export default {
  name: 'HomeView',
  components: {
    HelloI18n
  }
}
</script>
