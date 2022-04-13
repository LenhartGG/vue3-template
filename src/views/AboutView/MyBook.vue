<template>
  <div>{{ collectionName }}: {{ readersNumber }} {{ book.title }}</div>
</template>

<script>
  import { onMounted, ref, reactive } from 'vue'

  export default {
    props: {
      collectionName: String
    },
    setup(props, context) {
      
      // mounted
      onMounted(() => {
        console.log('Component is mounted!')
      })
      console.log(props, context);
      console.log(props.collectionName, context);
      const readersNumber = ref(0)
      const book = reactive({ title: 'Vue 3 Guide' })

      // 暴露给 template
      return {
        readersNumber,
        book
      }
    }
  }
</script>