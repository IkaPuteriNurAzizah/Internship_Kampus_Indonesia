<template>
  <div>
    <b-navbar toggleable="lg" type="light" fixed="top" class="nav">
      <div class="container">
        <b-navbar-brand href="#"
          ><img src="../assets/images/KampusIndonesia.png" alt=""
        /></b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <li class="nav-item">
              <router-link class="nav-link kiri" to="/">
                <p>Beranda</p>
              </router-link>
            </li>
            <b-nav-item-dropdown class="kiri kiri2" text="Fitur" right>
              <b-dropdown-item href="#"
                ><router-link class="nav-link" to="/list1"
                  >Cari Kampus/Prodi</router-link
                ></b-dropdown-item
              >
              <b-dropdown-item href="#"
                ><router-link class="nav-link" to="/"
                  >Cari Seminar/Workshop</router-link
                ></b-dropdown-item
              >
              <b-dropdown-item href="#"
                ><router-link class="nav-link" to="/"
                  >Cari Beasiswa</router-link
                ></b-dropdown-item
              >
              <b-dropdown-item href="#"
                ><router-link class="nav-link" to="/"
                  >Cari Lomba</router-link
                ></b-dropdown-item
              >
              <b-dropdown-item href="#"
                ><router-link class="nav-link" to="/"
                  >Cari Lowongan</router-link
                ></b-dropdown-item
              >
              <b-dropdown-item href="#"
                ><router-link class="nav-link" to="/"
                  >UTBK</router-link
                ></b-dropdown-item
              >
            </b-nav-item-dropdown>
            <li class="nav-item">
              <router-link class="nav-link kiri" to="/">
                <p>Hubungi Kami</p>
              </router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link kiri" to="/">
                <p>Blog</p>
              </router-link>
            </li>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <li class="nav-item">
              <router-link id="button" class="nav-link kanan" to="/">
                <p>Masuk</p>
              </router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link kanan daftar" to="/">
                <p>Daftar</p>
              </router-link>
            </li>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style></style>