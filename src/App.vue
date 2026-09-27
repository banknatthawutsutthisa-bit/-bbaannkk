<template>
  <div id="app">

    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">

        <router-link class="navbar-brand" to="/">
          Navbar
        </router-link>

        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div
          class="collapse navbar-collapse"
          id="navbarNavDropdown"
        >
          <ul class="navbar-nav">

            <!-- Home -->
            <li class="nav-item">
              <router-link
                class="nav-link"
                to="/"
                exact-active-class="active"
              >
                Home
              </router-link>
            </li>

            <!-- About -->
            <li class="nav-item">
              <router-link
                class="nav-link"
                to="/about"
                exact-active-class="active"
              >
                About
              </router-link>
            </li>

            <!-- Contact -->
            <li class="nav-item">
              <router-link
                class="nav-link"
                to="/contact"
                exact-active-class="active"
              >
                Contact
              </router-link>
            </li>

            <!-- Dropdown -->
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Dropdown link
              </a>

              <ul class="dropdown-menu">
                <li>
                  <a class="dropdown-item" href="#">
                    Action
                  </a>
                </li>

                <li>
                  <a class="dropdown-item" href="#">
                    Another action
                  </a>
                </li>

                <li>
                  <a class="dropdown-item" href="#">
                    Something else here
                  </a>
                </li>
              </ul>
            </li>

          </ul>
        </div>
      </div>
    </nav>

    <!-- เนื้อหาหน้าเว็บ -->
    <main class="page-content">
      <router-view />
    </main>

    




  </div>
</template>

