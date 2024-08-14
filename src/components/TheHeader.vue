<template>
  <header>
    <div class="displayHeader">
    <h1 :class="classVar">to-do list</h1>
    <div>
    <label>User</label>
    <input 
    v-model="name"
    type="text">
    {{ name }}
  </div>
  </div>
  </header>


</template>

<script>
export default {
  name: "TheHeader", // Nome do componente corrigido
  data() {
    return {
      name: 'joao',
      classVar: "title",
    };
  },
};
</script>

<style>
* {
  border-radius: 5px;
}
header {
  color: white;
  padding: 0.5rem;
  margin-bottom: 5px;
}

.todos {
  background: rgb(26, 26, 26);
  color: white;
  padding: 0.5rem;
  margin-bottom: 5px;
}

.img {
  width: 45px;
}

.title {
  color: rgb(91, 42, 226);
  margin: 0;
}

.displayHeader {
  justify-content: space-between;
  display: flex;
}
</style>
