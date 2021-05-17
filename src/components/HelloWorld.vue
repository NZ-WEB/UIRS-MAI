<template>
  <div>
    <iframe class="window" src="http://tm.spbstu.ru/htmlets/Degterev/WebGL/pr/interface.html"
            frameborder="0"></iframe>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
*{
  box-sizing: border-box;
}

.menu__list-item + .menu__list-item  {
  margin-left: 24px;
}


.window {
  width: 100%;
  height: 500px;
}
</style>
