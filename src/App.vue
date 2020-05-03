<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Huấn và Châm</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  #nav {
    a {
      font-size: 2rem;
      font-weight: bold;
      text-decoration: none;
    }
  }
}
</style>
