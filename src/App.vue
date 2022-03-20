<template>
  <div id="app">
    <div class="navbar-container">
      <div class="navbar-content">
        <router-link to="/">
          <i class="bx bx-home bx-sm"></i>
        </router-link>
        <router-link to="/cesta">
          <i class="bx bxs-message-square-dots bx-sm"></i>
        </router-link>
        <router-link to="/favoritos">
          <i class="bx bx-heart bx-sm"></i>
        </router-link>
        <router-link to="/historial">
          <i class="bx bx-revision bx-sm"></i>
        </router-link>
      </div>
    </div>

    <router-view />
  </div>
</template>

<style >

* {
  margin: 0px;
  padding: 0px;
  font-family: 'Fredoka One', cursive;
  font-family: 'Oswald', sans-serif;
  

}

.navbar-container {
  width: 100%;
  position: fixed;
  bottom: 0%;

  /* background-color: red;*/
}
.navbar-content {
  padding: 10px;
  display: flex;
  justify-content: space-between;
  color: aliceblue;
}

a {
  padding: 20px;
}
.navbar-content a {
  color: rgb(106, 112, 85);
}
.navbar-content a:hover {
  color: rgb(117, 145, 17);
}

.navbar-content a:router-link-exact-active {
  color: rgb(76, 10, 199);
}

a:-webkit-any-link {
  color: webkit-link;
  cursor: pointer;
  text-decoration: underline;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}



</style>
