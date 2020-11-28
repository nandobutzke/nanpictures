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
      photos: []
    }
  },
  created() {
    alert('Um componente foi criado')
  }
}

</script>

<style>
</style>
