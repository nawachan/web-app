<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">ありがとう…ッッ！</button>
    <p>
      ありがとうと思った数だけボタンを押しましょう。
    </p>
  </div>

  <p>
    あなたは今日 {{ count }} 回感謝しました。
  </p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
