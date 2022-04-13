<template>
  <div>
    <h2>TodoListStatistics</h2>
    inject: {{ user }} <br/>
    数量： {{ todoLength }}
    <!-- 模板的其余部分 -->
  </div>
</template>

<script>
export default {
  inject: ['user', 'todoLength'],
}
</script>

<style>

</style>