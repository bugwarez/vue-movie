<template>
  <header>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <!-- Container wrapper -->
      <div class="container mb-2">
        <!-- Navbar brand -->
        <router-link to="/">
          <img
            class="img-fluid logo mt-2"
            src="./assets/img/what_to_watch_logo.png"
          />
        </router-link>
        <!-- Toggle button -->
        <button
          class="navbar-toggler"
          type="button"
          data-mdb-toggle="collapse"
          data-mdb-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <fa icon="fas fa-bars" />
        </button>

        <!-- Collapsible wrapper -->
        <div class="collapse navbar-collapse">
          <!-- Left links -->
          <ul class="navbar-nav mx-2 mt-2">
            <li class="nav-item">
              <a
                class="nav-link active d-flex align-items-center"
                aria-current="page"
                href="#"
              >
                <i class="fas fa-bars pe-2"></i>Menu
              </a>
            </li>
          </ul>
          <!-- Left links -->

          <form class="d-flex align-items-center w-100 form-search">
            <div class="input-group">
              <button
                class="btn btn-light dropdown-toggle shadow-0 mt-2"
                type="button"
                data-mdb-toggle="dropdown"
                aria-expanded="false"
                style="padding-bottom: 0.4rem"
              >
                All
              </button>
              <ul class="dropdown-menu dropdown-menu-dark fa-ul">
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2">
                      <i class="fas fa-search"></i> </span
                    >All
                  </a>
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2"> <i class="fas fa-film"></i> </span
                    >Titles
                  </a>
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2"> <i class="fas fa-tv"></i> </span
                    >TV Episodes
                  </a>
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2">
                      <i class="fas fa-user-friends"></i> </span
                    >Celebs
                  </a>
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2">
                      <i class="fas fa-building"></i> </span
                    >Companies
                  </a>
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2"> <i class="fas fa-key"></i> </span
                    >Keywords
                  </a>
                </li>
                <li>
                  <hr class="dropdown-divider" />
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <span class="fa-li pe-2">
                      <i class="fas fa-search-plus"></i> </span
                    >Advanced search
                    <i class="fas fa-chevron-right ps-2"></i>
                  </a>
                </li>
              </ul>
              <input
                type="search"
                class="form-control mt-2"
                placeholder="Search"
                aria-label="Search"
              />
            </div>
            <a href="#!" class="text-white">
              <i class="fas fa-search ps-3"></i>
            </a>
          </form>

          <ul class="navbar-nav">
            <li class="nav-item mt-2 mx-2">
              <a class="nav-link d-flex align-items-center" href="/watchlist">
                <fa icon="bookmark" />&nbsp;Watchlist
              </a>
            </li>
            <li class="nav-item mt-2 mx-2">
              <a class="nav-link d-flex align-items-center" href="/login">
                <fa icon="right-to-bracket" />&nbsp;Login
              </a>
            </li>
          </ul>
        </div>
        <!-- Collapsible wrapper -->
      </div>
      <!-- Container wrapper -->
    </nav>
    <!-- Navbar -->
  </header>
  <main>
    <router-view />
  </main>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Fira+Sans:wght@400&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Fira Sans", sans-serif;

  &::selection {
    background: transparentize(#f5c518, 0.5);
  }
}

body {
  background-color: #343a40 !important;
}
a {
  text-decoration: none;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  color: #fff;
}

.logo {
  width: 16vw;
}

.navbar-dark .nav-item .nav-link {
  color: #fff;
}

.navbar-dark .nav-item .nav-link:hover {
  background-color: rgba(255, 255, 255, 0.1);
  transition: all 0.3s ease;
  border-radius: 0.25rem;
  color: #fff;
}

.fa-li {
  position: relative;
  left: 0;
}
.video_card {
  background-color: #343a40 !important;
  color: #fff !important;
}
.n-card.n-card--bordered {
  border: 0 !important;
}
.n-card-header__main {
  font-size: 1.6em;
  color: #fff !important;
  margin: 0 !important;
  padding: 0 !important;
}
</style>
