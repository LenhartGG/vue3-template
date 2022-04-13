<template>
  <div>
    <!-- 模板的其余部分 -->
    <h2>TodoListFooter</h2>
    inject: {{ user }} <br/>
    数量： {{ todoLength }}

    <TodoListStatistics />
  </div>
</template>

<script>
import TodoListStatistics from './TodoListStatistics'
export default {
  components: {
    TodoListStatistics,
  },
  inject: ['user', 'todoLength'],
  data() {
    return {
    }
  },
}
</script>

<style>

</style>