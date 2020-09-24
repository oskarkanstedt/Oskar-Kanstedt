<template>
  <div id="app">
    My repos:
    <ul>
      <!-- Här loopar vi ut this.repos -->
      <li v-for="repo in repos" :key="repo.name">{{ repo.name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      repos: [], // initiera this.repos som en tom array
    }
  },
  async mounted() {
    const result = await fetch(
      'https://api.github.com/users/oskarkanstedt/repos'
    )
    const json = await result.json()
    this.repos = json // sätt this.repos till datan vi hämtat
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
