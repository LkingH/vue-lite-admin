<template>
  <resize-box>
    <template #left>
      <h2>在左侧输入框输入标签，右侧实时将微信渲染成img标签</h2>
      <el-input
        type="textarea"
        :rows="4"
        placeholder="请输入内容"
        v-model="text1"
      />
      <emotion-box position="top" @emotion-add="(e) => (text1 += e)" />
    </template>
    <template #right>
      <div v-html="processText" />
    </template>
    <template #line>
      <app-icon icon="el-icon-right" />
    </template>
  </resize-box>
  <compare-box/>
</template>

<script>
import EmotionBox from '/src/components/EmotionBox/index.vue'
import CompareBox from '/src/components/CompareBox/index.vue'
import ResizeBox from '/src/components/ResizeBox/index.vue'
import { useProcessEmotion } from '/src/components/EmotionBox/useEmotions'
import { computed, ref } from 'vue'
export default {
  name: 'EmotionDemo',
  components: { EmotionBox, ResizeBox,CompareBox },
  setup() {
    const text1 = ref('')
    const processText = computed(() => useProcessEmotion(text1.value))
    return { text1, processText }
  },
}
</script>

<style lang="scss" scoped></style>
