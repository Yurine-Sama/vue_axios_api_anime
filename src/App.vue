<template>
  <div id="app">
    <b-navbar toggleable="lg" type="dark" variant="danger">
      <img
        src="https://i.redd.it/vvuxyi4qadf41.jpg"
        alt="อามิยะกำหมัดแล้วน้าาา"
        width="80px"
        height="75px"
      />
      <h1 style="color: white;">ANIME</h1>
    </b-navbar>
    <router-view style="margin-top: 30px" />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
