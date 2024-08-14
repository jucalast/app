<template>
  <div>
    <div v-for="(obj, index) in todos" :key="obj.id" class="todos">
      <img v-if="obj.imgSrc" :src="obj.imgSrc" :alt="imgAlt" class="img" />
      {{ index }} - {{ obj.title }}
    </div>
  </div>
</template>

<script>
export default {
  name: "TheList", // Nome do componente corrigido
  data() {
    return {
      classVar: "title",
      imgAlt: "imagem",
      todos: [
        // Certifique-se de que o array está bem definido
        {
          userId: 1,
          id: 1,
          title: "delectus aut autem",
          completed: false,
          imgSrc: "https://via.placeholder.com/600/92c952",
        },
        {
          userId: 1,
          id: 2,
          title: "quis ut nam facilis et officia qui",
          completed: false,
        },
        { userId: 1, id: 3, title: "fugiat veniam minus", completed: false },
        {
          userId: 1,
          id: 4,
          title: "et porro tempora",
          completed: true,
          imgSrc: "https://via.placeholder.com/600/92c952",
        },
        {
          userId: 1,
          id: 5,
          title:
            "laboriosam mollitia et enim quasi adipisci quia provident illum",
          completed: false,
        },
        {
          userId: 1,
          id: 6,
          title: "delectus aut autem",
          completed: false,
          imgSrc: "https://via.placeholder.com/600/92c952",
        },
        {
          userId: 1,
          id: 7,
          title: "quis ut nam facilis et officia qui",
          completed: false,
        },
        { userId: 1, id: 8, title: "fugiat veniam minus", completed: false },
        { userId: 1, id: 9, title: "et porro tempora", completed: true },
        {
          userId: 1,
          id: 10,
          title:
            "laboriosam mollitia et enim quasi adipisci quia provident illum",
          completed: false,
        },
      ],
    };
  },
};
</script>
