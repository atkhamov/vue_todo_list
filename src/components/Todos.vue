// Start TEMPLATE
<template>
   <div>
      <div v-for-key="todo in todos">
         <h3>{{todo.title}}</h3>
      </div>
   </div>
</template>

// Start SCRIPT
<script>
export default {
   name: "Todos",
   props: ["todos"]
}
</script>

// Start STYLE
<style scoped>

</style>