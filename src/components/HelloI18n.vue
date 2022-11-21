<template lang="pug">
.hello
  h2 {{ t('xiao') }}
  img.main(src="https://scontent.ftpe7-1.fna.fbcdn.net/v/t1.18169-9/20429797_10155277993756208_4109811426447335948_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=ybnnqyrQI_gAX89a0qB&_nc_ht=scontent.ftpe7-1.fna&oh=00_AfD1GgTwhdh8pHNyLDqGkluFJNpr0JRu8y85xIVLUlNsEA&oe=63A26991", alt="main")

</template>

<script>
import { defineComponent } from 'vue'
import { useI18n } from 'vue-i18n'

export default defineComponent({
  name: 'HelloI18n',
  setup() {
    const { t } = useI18n({
      inheritLocale: true,
      useScope: 'local'
    })

    return { t }
  }
})
</script>

<style type="text/css" scoped>
  .main {
    width: 33vw;
  }
</style>
