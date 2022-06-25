<template>
  <div id="app">
    <ul>
      <li v-for="(item, index) in items" :key="index">
        {{ (index + 1) }}. {{ item.nama }} - Status : {{ item.stok > 1 ? "Tersedia" :
        "Habis"
        }}
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      items: [
        { nama: "Apel", stok: "500" },
        { nama: "Mangga", stok: "100" },
        { nama: "Jeruk", stok: "0" },
      ]
    }
  },
  // components: {
  //   HelloWorld
  // }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
