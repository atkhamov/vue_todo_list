// Start TEMPLATE
<template>
   <div>
      <div v-bind:key="todo.id" v-for="todo in todos">
         <TodoItem v-bind:todo="todo" v-on:del-todo="$emit('del-todo', todo.id)"/>
      </div>
   </div>
</template>

// Start SCRIPT
<script>
import TodoItem from './TodoItem.vue';
export default {
   name: "Todos",
   components:{
      TodoItem
   },
   props: ["todos"]
}
</script>

// Start STYLE
<style scoped>

</style>