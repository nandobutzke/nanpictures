<template>
  <div>
    <h1>{{ title}}</h1>

    <ul>
      <li v-for="photo of photos">
        <img :src="photo.url" :alt="photo.titulo">
      </li>
    </ul>

  </div>
</template>

<script>
export default {
  data() {
    return {

      title: 'Alurapic', 
      photos: [
        {
          url: 'http://tudosobrecachorros.com.br/wp-content/uploads/cachorro-independente.jpg',
          titulo: 'cachorro'
        },
        {
          url: 'http://tudosobrecachorros.com.br/wp-content/uploads/cachorro-independente.jpg',
          titulo: 'Cachorrão'
        }
      ]
    }
  }
}

</script>

<style>
</style>
