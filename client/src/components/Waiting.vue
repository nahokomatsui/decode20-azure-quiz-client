<template>
  <v-container>
    <v-row
      justify="center"
    >
      <v-col cols="12" lg="6" md="6" sm="12" xs="12">
        夏まつりクイズへようこそ！
      </v-col>
    </v-row>
    <v-row
      justify="center"
    >
      <v-col cols="12" lg="6" md="6" sm="12" xs="12" class="text-left">
        <v-card class="mx-auto" max-width="600">
          <v-card-title>
            使い方
          </v-card-title>
          <v-card-text>
            <ol>
              <li>司会の操作により質問表示画面、回答画面が自動的に切り替わります。</li>
              <li>回答画面では、正しいと思う答えを選択し、回答を送信してください。</li>
            </ol>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-row
      justify="center"
    >
      <v-col cols="12" lg="6" md="6" sm="12" xs="12">
        あなたの ID は <code>{{ uuid }}</code>
      </v-col>
    </v-row>
    <v-row class="text-center">
      <v-col>
        <v-btn @click="$emit('reset-results')">Rest results</v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'Waiting',
  props: {
    uuid: String,
  },
});
</script>
