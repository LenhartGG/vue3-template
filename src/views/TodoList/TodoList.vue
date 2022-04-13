<template>
  <div>
    provide: {{user}}
    数量：{{ todos.length }}
    <!-- 模板的其余部分 -->
    <div v-for="(item, index) in todos" :key="index">
      <TodoItem :item="item"/>
    </div>
    <TodoListFooter />
  </div>
</template>

<script>
import TodoItem from './TodoItem'
import TodoListFooter from './TodoListFooter'
export default {
  components: {
    TodoItem,
    TodoListFooter,
  },
  data() {
    return {
      user: 'John Doe',
      todos: ['Feed a cat', 'Buy tickets']
    }
  },
  provide() {
    return {
      user: this.user,
      todoLength: this.todos.length
    }
  },
}
</script>

<style>

</style>