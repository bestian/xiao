<template lang="pug">
.about
  h2 {{$t('about_me')}}
  .ui.grid.container
    .row
      .eight.wide.column
        img.main(src="https://scontent.ftpe7-1.fna.fbcdn.net/v/t1.18169-9/20429797_10155277993756208_4109811426447335948_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=ybnnqyrQI_gAX89a0qB&_nc_ht=scontent.ftpe7-1.fna&oh=00_AfD1GgTwhdh8pHNyLDqGkluFJNpr0JRu8y85xIVLUlNsEA&oe=63A26991", alt="main")
      .eight.wide.column.ui.segment
        p 友善蔬食料理
        p 台灣咖啡 茶
        p 手作特色甜點
        p 料理教學
        p 供餐時間：週四 - 六 12:00-20:30（中間無休息，L.O. 19:30）
        p 週日 - 三 舉行料理課程 / 各式活動與場地租借
        hr
        p.note ※ 如需包場用餐，或客製包班課程，請另私訊安排
</template>

<style type="text/css" scoped>
  .main {
    width: 100%;
  }
</style>
