<template>
  <section class="home">
    <Navbar />

    <div class="container">
      <Hero />

      <div class="row mt-4">
        <div class="col">
          <h3>
            <strong>Rekomendasi Kampus Terbaik</strong>
          </h3>
        </div>
        <div class="col">
          <router-link to="/list1" class="btn btn-primary float-right">
            <b-icon-eye></b-icon-eye> Lihat Semua
          </router-link>
        </div>
      </div>

      <div class="row mb-4">
        <div
          class="col-md-4 mt-4"
          v-for="product in products"
          :key="product.id"
        >
          <Kampus :product="product" />
        </div>
      </div>
    </div>

    <Lokasi />

    <Fitur />

    <div class="container">
      <Lowongan />

      <Seminar1 />

      <Artikel />
    </div>

    <Partner />
  </section>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Hero from "@/components/Hero.vue";
import Kampus from "@/components/Kampus.vue";
import Lokasi from "@/components/Lokasi.vue";
import Fitur from "@/components/Fitur.vue";
import Lowongan from "@/components/Lowongan.vue";
import Seminar1 from "@/components/Seminar1.vue";
import Artikel from "@/components/Artikel.vue";
import Partner from "@/components/Partner.vue";
import axios from "axios";

export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    Kampus,
    Lokasi,
    Fitur,
    Lowongan,
    Seminar1,
    Artikel,
    Partner,
  },
  data() {
    return {
      products: [],
    };
  },
  methods: {
    setProducts(data) {
      this.products = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3000/best-products")
      .then((response) => this.setProducts(response.data))
      .catch((error) => console.log(error));
  },
};
</script>