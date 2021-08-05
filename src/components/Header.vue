<template>
  <header>
    <h1>{{ title }}</h1>
    <Button />
  </header>
</template>

<script>
import Button from './Button.vue'

export default {
  name: 'Header',
  // props: ['title'], => declare props in an array
  props: {
    title: String,
    // title: {
    //   type: String,
    //   default: 'Hello Vue.js'
    // }
  },
  components: {
    Button
  }
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>