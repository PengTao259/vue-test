<template>
  <div id="app">
    <!-- 默认插值 -->
    <StudyM title="游戏列表">
      <ul>
        <li v-for="game, index in games" :key="index">{{ game }}</li>
      </ul>
    </StudyM>
    <StudyM title="推荐音乐">
      <ul>
        <li v-for="music, index in musics" :key="index">{{ music }}</li>
      </ul>
    </StudyM>
    <StudyM title="电影推荐">
      <ul>
        <li v-for="movie, index in movies" :key="index">{{ movie }}</li>
      </ul>
    </StudyM>
  </div>
</template>

<script>
export default {
  data () {
    return {
      games: ['英雄联盟', '炉石传说', '穿越火线', 'QQ飞车', '吃鸡'],
      musics: ['迷途羔羊', '红玫瑰', '富士山下', '麻雀', '妈妈的话', '故乡'],
      movies: ['蜘蛛侠', '复仇者联盟', '金刚狼', '触不可及', '唐人街探案', '当幸福来敲门']
    }
  }
}
</script>

