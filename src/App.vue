<template>
  <div id="app">
    <nav id="nav" class="navbar navbar-expand-lg navbar-light">

    <a class="navbar-brand" href="#">
      <img src="@/assets/ebeauty.png" alt="" height="24" class="d-inline-block align-text-top"/>
      
    </a>

    <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarToggler"
        aria-controls="navbarToggler"
        aria-expanded="false"
        aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
      </button>

    <div class="collapse navbar-collapse" id="navbarToggler">
      <ul class="navbar nav mr-auto mt-2 mt-lg-0">
        <li class="nav-item">
            <router-link to="/" class="nav-link">Home</router-link>
        </li>
        <li class="nav-item">
            <router-link to="/gallery" class="nav-link">Gallery</router-link>
        </li>
        <li class="nav-item">
            <router-link to="/login" class="nav-link">Log in</router-link>
        </li>
        <li class="nav-item">
            <router-link to="/signup" class="nav-link">Sign up</router-link>
        </li>
      </ul>
     
    </div>
   </nav>
      <div class="container-fluid">
      <router-view/>
      </div>
     
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1f2429;
}

#nav {
  width: 100%;
  padding: 10px;
  background-color: white;
  position: fixed;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #dd6f6b;
    }
  }
}


#title {
  font-family: 'Montserrat';
}

#prvigrid {

  background-color: rgb(208, 162, 128);
}

body {
  background-color: rgb(208, 162, 128);
}

#datum {
  margin-top: 100px;
}

#galerija {
  position: inherit;
}

</style>
