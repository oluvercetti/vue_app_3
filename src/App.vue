<template>
  <div id="app">
    <header id="header">
      <span id="title">Header Set in App.vue</span>
      <div id="nav">
        <router-link to="/">Introduction</router-link> |
        <router-link to="/spec">Tech Spec</router-link> |
        <router-link to="/history">History</router-link>
      </div>
    </header>
    <main id="main">
    </main>
    <router-view/>
    <footer id="footer">
      <span id="title">Footer Set in App.vue</span>
    </footer>

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

#header {
  position: fixed;
  top: 0;
  left: 0;
  height: 45px;
  width: 100%;
  background: red;
}

#title {
  font-size: 22px;
  color: white;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}

#main {
  padding-top: 45px;
  padding-bottom: 50px;
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

#footer {
  position: fixed;
  bottom: 0;
  left: 0;
  height: 45px;
  width: 100%;
  background: red;
}
</style>
