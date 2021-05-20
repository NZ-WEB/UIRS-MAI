<template>
  <v-container>
    <v-row class="flex-column justify-center align-items-center mt-5">
      <v-col class="col-9">
        <img src="../assets/main.svg" alt="" class="main-img">
      </v-col>
      <v-col class="col-9 mt-5">
        <h1 class="main-title">
          Three.js в деле!
        </h1>
        <p class="main-description pt-2 pb-2">
          На данном сервисе продемонстрирована визуализация механической системы
        </p>
        <router-link to="system" class="main-btn">
          <v-btn
              elevation="1"
              x-large
              class="mt-2"
              color="#3F51B5"
          >
            <span style="color:#fff; text-transform: none; font-weight: 500; text-decoration: none">Перейти к системе</span>
          </v-btn>
        </router-link>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({}),
}
</script>

<style scoped lang="scss">


.window {
  width: 800px;
  height: 500px;
}

.main {

  &-btn {
    text-align: center;
    margin: 0;
  }

  &-title {
    font-size: 60px;
    font-weight: bold;
  }

  &-description {
    max-width: 460px;
    margin: 0 auto;
  }


  &-img {
    width: 100%;
  }
}

@media (max-width: 650px) {
  h1 {
    font-size: 40px;

  }
  p {
    font-size: 18px;
  }
}


</style>
