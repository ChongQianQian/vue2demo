<template>
  <div>
    <input :value="value" @input="onInputChange" v-bind="$attrs" autocomplete="off"/>
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      default: '我是子组件默认的props数据'
    }
  },
  methods: {
    onInputChange (e) {
      this.$emit('input', e.target.value)
    }
  }
}
</script>

<style scoped>
</style>
