<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <a class="nav-link" href="/"
              >Home <span class="sr-only">(current)</span></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="reviews">Reviews</a>
          </li>
        </ul>
      </div>
    </nav>
    <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav> -->
    <router-view />
    <footer class="bg-light text-center text-lg-start">
      <!-- Copyright -->
      <div
        class="text-center p-3"
        style="
          display: flex;
          justify-content: center;
          background-color: rgba(0, 0, 0, 0.2);
        "
      >
        GITHUB->
        <a
          class="text-dark"
          href="https://github.com/BYUCS260/xkcd-browser-jacobthecanopier"
        >
          https://github.com/jacobthecanopier/cp3</a
        >
      </div>
      <!-- Copyright -->
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

nav {
  font-size: 25px;
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
