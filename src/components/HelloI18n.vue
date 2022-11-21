<template lang="pug">
.hello
  h2 {{ $t('xiao') }}
  .ui.grid.container
    .row
      .eight.wide.column
        img.main(src="https://scontent.ftpe7-3.fna.fbcdn.net/v/t39.30808-6/296070488_2348801425277541_1145109733943763674_n.jpg?stp=cp6_dst-jpg_s960x960&_nc_cat=102&ccb=1-7&_nc_sid=e3f864&_nc_ohc=-9u6k-xMpAEAX_k_dmU&tn=IC4WyFbFWgekXOS9&_nc_ht=scontent.ftpe7-3.fna&oh=00_AfA0wGT4H75dAriENREQQenQ9SB4P3PfxVAejcGS3kYEyA&oe=637F50A1", alt="place")
        img.main(src="https://scontent.ftpe7-1.fna.fbcdn.net/v/t31.18172-8/28424411_954121691412195_2303959143217582318_o.jpg?_nc_cat=106&ccb=1-7&_nc_sid=e3f864&_nc_ohc=imWIC6e_8ZYAX8-9LSf&_nc_ht=scontent.ftpe7-1.fna&oh=00_AfASvw5ksvKSKC6DOIurd7Y6dMwWszRXPrgFnKw9I5sL3Q&oe=63A25959", alt="work")
      .eight.wide.column
        img.main(src="https://scontent.ftpe7-1.fna.fbcdn.net/v/t39.30808-6/298564404_2360263740797976_7403381146999988939_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=c4c01c&_nc_ohc=syKoSZu9EZ4AX_-3ka5&_nc_ht=scontent.ftpe7-1.fna&oh=00_AfD7g7WVbChrDIAcn4tEDP6c_lplsfkMdi7NIpphW-W80Q&oe=63802416", alt="menu")
        img.main(src="https://scontent.ftpe7-4.fna.fbcdn.net/v/t39.30808-6/298528879_2360263824131301_3281003154184598208_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=c4c01c&_nc_ohc=GpNAdsWRMI4AX8ikccb&_nc_ht=scontent.ftpe7-4.fna&oh=00_AfCqDak9RPmco1iZCJthc96YZn2V2kXX_3vMGWz_5Jy24g&oe=637F4BC6", alt="menu2")
        img.main(src="https://scontent.ftpe7-4.fna.fbcdn.net/v/t39.30808-6/298508265_2360263887464628_826021878921983093_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=c4c01c&_nc_ohc=EvUsVeDkgs4AX8CuKt9&_nc_ht=scontent.ftpe7-4.fna&oh=00_AfBok7QAQJ3oB-uenL51QODQUxu-b3qDlUiwMSq5jOAMWw&oe=637F1CEB", alt="menu3")

</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'HelloI18n'
})
</script>

<style type="text/css" scoped>
  .main {
    width: 100%;
  }
</style>
