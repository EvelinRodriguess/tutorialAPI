<script setup>
// import { ref, onMounted } from 'vue'
// import api from '@/plugins/axios'

// const moviesGenres = ref([])
// const TVGenres = ref([])

// onMounted(async () => {
//   let response = await api.get('genre/movie/list?language=pt-BR')
//   moviesGenres.value = response.data.genres
//   response =  await api.get('genre/tv/list?language=pt-BR')
//   TVGenres.value = response.data.genres
// })
// </script>

<template>
  


  <template>
  <header>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/filmes">Filmes</router-link>
      <router-link to="/tv">Programas de TV</router-link>
    </nav>
  </header>
  <main>
    <router-view />
  </main>
</template>
</template>


<style scoped>
nav {
  display: flex;
  justify-content: flex-start;
  margin-bottom: 1rem;
  column-gap: 2rem;
}


header {
  height: 3rem;
  display: flex;
  background-color: black;
  color: #fff;
  font-size: 1.2rem;
  padding-left: 2rem;
}

nav {
  column-gap: 2rem;
  margin-bottom: 0;
  display: flex;
  align-items: center;
}

nav a {
  text-decoration: none;
  color: #fff;
}
</style>