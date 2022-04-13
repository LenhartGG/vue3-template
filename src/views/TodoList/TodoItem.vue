<template>
  <div>
    {{item}}
    <!-- 模板的其余部分 -->
  </div>
</template>

<script>
export default {
  props: ['item'],
  data() {
    return {
      todos: ['Feed a cat', 'Buy tickets']
    }
  },
}
</script>

<style>

</style>