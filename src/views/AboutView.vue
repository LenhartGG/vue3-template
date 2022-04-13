<template>
  <div class="about">
    <h1>This is an about page</h1>
    <MyBook :collectionName="collectionName"/>
    <h2>TodoList</h2>
    <TodoList />
  </div>
</template>

<script>
import MyBook from './AboutView/MyBook.vue';
import TodoList from './TodoList/TodoList.vue';
export default {
  components: {
    MyBook,
    TodoList,
  },

  data() {
    return {
      collectionName: 'collectionName'
    };
  },

  mounted() {
    
  },

  methods: {

  },
};
</script>

<style lang="less" scoped>

</style>