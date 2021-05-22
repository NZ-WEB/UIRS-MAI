<template>
  <div class="about">
    <h3 class="mb-5">
      Описание front-end части
    </h3>
    <p class="post mb-5">
      SPA построен на басе Vue.js. Сборка была произведена при помощи vue.cli. Также для роутинга внутри приложения был использован функционал vue-router, обеспечивающий роутинг между страницами без их перезагрузки.
      UI - составляющая была реализована при помощи библиотеки Vuetiffy.
      <br>
      Сама Система была построена при помощи фреймворка Three.js. И интеграцией библиотеки с реализацией мониторинга fps, нагрузки системы и статистики.
      Интеграция системы была произведена через "iframe".
    </p>
    <h3 class="mb-5">
      Описание системы
    </h3>
    <p class="post" v-for="post in allPosts" :key="post.id">
      <i>
        {{ post.body }}
      </i>
    </p>
  </div>
</template>
<script>
import {mapGetters, mapActions} from 'vuex'
export  default {
  data() {
    return {
    }
  },
  methods: mapActions(['fetchPosts']),

  // 1rst methood
  // computed: {
  //   allPosts() {
  //     return this.$store.getters.allPosts;
  //   }
  // },
  //2nd methood
  computed: mapGetters(['allPosts']),
  //default fetch request
  // async mounted() {
  //   const res = await fetch(
  //       'https://jsonplaceholder.typicode.com/posts?_limit=1'
  //   );
  //   const posts = await res.json();
  //   this.posts = posts;
  // }
  async mounted() {
    //this.$store.dispatch('fetchPosts'); default method
    this.fetchPosts(5)
  }
}
</script>

<style scoped lang="scss">

.post {
  max-width: 700px;
  width: 100%;
  margin: 0 auto;
}


</style>
