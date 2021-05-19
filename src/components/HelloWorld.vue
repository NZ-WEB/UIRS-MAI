<template>
  <v-container>
    <v-row>
      <div class="pt-5 mx-auto">
        <iframe class="window" src="http://tm.spbstu.ru/htmlets/Degterev/WebGL/pr/interface.html"
                frameborder="0"></iframe>
      </div>
    </v-row>
    <v-row justify="center">
      <v-col>
        <div class="text-center">
          <v-dialog
              v-model="dialog"
              width="500"
          >
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                  color="red lighten-2"
                  dark
                  v-bind="attrs"
                  v-on="on"
              >
                Click Me
              </v-btn>
            </template>

            <v-card>
              <v-card-title class="headline grey lighten-2">
                Описание задания
              </v-card-title>

              <v-card-text>
                Текст описания текст описания текст описания текст описания
              </v-card-text>

              <v-divider></v-divider>

              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn
                    color="primary"
                    text
                    @click="dialog = false"
                >
                  Закрыть
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-dialog>
        </div>
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

</style>
