<template>
  <div class="video-player">
    <div class="video-list">
      <div :key="video.id" v-for="video in videos" class="thumbnail">
        <div class="thumbnail-img">
          <img :src="video.thumbnail" />
        </div>
        <div class="thumbnail-info">
          <h3> {{video.title}} </h3>
          <p> {{video.creator}} </p>
          <p class="thumbnail-views"> {{video.views}} Views</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const videos = [
  {
    id: 1,
    title: 'Raw: Huge Crowd for Seahawks Parade in Seattle',
    thumbnail:
      'https://i.ytimg.com/an_webp/SUVFqvIKSDA/mqdefault_6s.webp?du=3000&sqp=CLm45tgF&rs=AOn4CLD2UGMNp7r-8SH7-XtOuZBxRAectA',
    youtubeURL: 'https://www.youtube.com/embed/SUVFqvIKSDA',
    creator: 'Associated Press',
    likes: 0,
    views: 0
  },
  {
    id: 2,
    title: 'The Legion of Boom',
    thumbnail:
      'https://i.ytimg.com/an_webp/P9LNSBqd1Fk/mqdefault_6s.webp?du=3000&sqp=CJiA5tgF&rs=AOn4CLCAVILm45tYOfLMk3I9BNOaCjnNig',
    youtubeURL: 'https://www.youtube.com/embed/P9LNSBqd1Fk',
    creator: 'Joseph Vincent',
    likes: 0,
    views: 0
  },
  {
    id: 3,
    title: 'Marshawn Lynch || "Beast Mode" ᴴᴰ || Seattle Seahawks Highlights',
    thumbnail:
      'https://i.ytimg.com/an_webp/eP8KXfB_zHg/mqdefault_6s.webp?du=3000&sqp=CJiA5tgF&rs=AOn4CLCmtgM97SH1OisDdUu8bvsuCe9YiQ',
    youtubeURL: 'https://www.youtube.com/embed/eP8KXfB_zHg',
    creator: 'TheGOON Productions',
    likes: 0,
    views: 0
  },
  {
    id: 4,
    title: '1995 ALDS Gm5: Ken Griffey Jr. scores the game-winning run to sends Mariners to ALCS',
    thumbnail:
      'https://i.ytimg.com/an_webp/F8SBJzOEcyU/mqdefault_6s.webp?du=3000&sqp=CJiA5tgF&rs=AOn4CLA7ZTnu2SXWM0NxuAZy-e7NOKRQuw',
    youtubeURL: 'https://www.youtube.com/embed/F8SBJzOEcyU',
    creator: 'MLB',
    likes: 788,
    views: 196076
  },
  {
    id: 5,
    title: 'Gary Payton - Sonic Pride',
    thumbnail:
      'https://i.ytimg.com/an_webp/i_a2KPCzKWw/mqdefault_6s.webp?du=3000&sqp=CJiA5tgF&rs=AOn4CLCFhkwkN9FUL62waTbnZQ1qg_R0ag',
    youtubeURL: 'https://www.youtube.com/embed/i_a2KPCzKWw',
    creator: 'Dunkman 827',
    likes: 917,
    views: 206059
  }
]

export default {
  name: 'VideoPlayer',
  data () {
    return {
      videos
    }
  }
}
</script>

<style scoped>

</style>
