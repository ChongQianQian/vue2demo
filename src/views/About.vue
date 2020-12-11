<template>
  <div>
    下面是v-model示例：
    <p>{{ pageTitle }}</p>

    下面是子组件内容：
    <ChildComponent v-model="pageTitle"  placeholder="今日待办" autofocus></ChildComponent>
  </div>
</template>

<script>
import ChildComponent from '@/components/ChildenComs/ChildComponent.vue'
export default {
  data () {
    return {
      pageTitle: '我是来自父组件的字符串'
    }
  },
  components: {
    ChildComponent
  }
}
</script>

<style scoped>
</style>
