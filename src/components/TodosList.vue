<template>
  <div>
    <todo v-for="(todo, index) in $store.state.todos" :key="index" :todo="todo" />
  </div>
</template>

<script>
import Todo from "./Todo";
export default {
  components: {
    Todo,
  },
  computed: {
    todos() {
      return this.$store.state.todos;
    },
  },
};
</script>

<style></style>
