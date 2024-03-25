<template>
  <section class="main-all">
    <header>
      <h1>TO DO LIST</h1>
    </header>
    <todo-list></todo-list>
  </section>
</template>

<script></script>

<style>
header {
  text-align: center;
}
body {
  font-family: sans-serif;
  display: flex;
  justify-content: center;
  background-color: rgb(255, 249, 241);
  color: rgb(255, 249, 241);
}
button {
  font-family: inherit;
  background-color: black;
  color: white;
  border: none;
  padding: 7px;
  margin-left: 5px;
  border-radius: 5px;
}

input {
  background-color: rgb(224, 191, 224);
  border: none;
  padding: 7px;
  border-radius: 5px;
}

.main-all {
  background-color: darkmagenta;
  padding: 40px;
  padding-top: 10px;
  margin-top: 200px;
  border-radius: 5px;
  border: 4px solid black;
}

ul {
  list-style: none;
  width: 100%;
  margin-right: 40px;
  padding: 0;
  text-align: center;
}

.main-todo {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
