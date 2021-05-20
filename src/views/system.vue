<template>
  <div>
    <iframe class="window" src="http://tm.spbstu.ru/htmlets/Degterev/WebGL/pr/interface.html" frameborder="0"></iframe>
  </div>
</template>

<style scoped lang="scss">

.window {
  width: 1000px;
  height: 600px;
}

@media (max-width: 1200px) {
  .window {
    width: 800px;
    height: 500px;
  }
}
@media (max-width: 1000px) {
  .window {
    width: 600px;
    height: 400px;
  }
}

@media (max-width: 860px) {
  .window {
    width: 500px;
    height: 300px;
  }
}

@media (max-width: 576px) {
  .window {
    width: 400px;
    height: 300px;
  }
}

@media (max-width: 420px) {
  .window {
    width: 300px;
    height: 250px;
  }
  .dg .main {
    max-width: 300px!important;
  }
}

</style>
