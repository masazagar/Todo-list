<template>
  <main class="main-todo">
    <form @submit.prevent="addTodo">
      <input type="text" v-model="input" />
      <button type="submit">Add todo</button>
    </form>

    <section class="todo-list">
      <ul v-for="(todo, index) in todos" :key="index">
        <li>{{ todo }} <button @click="deleteTodo(index)">X</button></li>
      </ul>
    </section>
  </main>
</template>

<script>
export default {
  data() {
    return {
      input: "",
      todos: [],
    };
  },
  methods: {
    addTodo() {
      this.todos.push(this.input);
      this.input = "";
    },
    deleteTodo(index) {
      this.todos.splice(index, 1);
    },
  },
};
</script>

<style>
/* body {
  font-family: sans-serif;
  display: flex;
  justify-content: center;
}

button {
  font-family: inherit;
} */
</style>
