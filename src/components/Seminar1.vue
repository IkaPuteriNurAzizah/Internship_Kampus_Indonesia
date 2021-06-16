<template>
  <div>
    <div class="row mt-4">
      <div class="col">
        <h3>
          <strong>Informasi Seminar</strong>
        </h3>
      </div>
      <div class="col">
        <router-link to="/" class="btn btn-primary float-right">
          <b-icon-eye></b-icon-eye> Lihat Semua
        </router-link>
      </div>
    </div>

    <div class="row mb-4">
      <div class="col-md-4 mt-4" v-for="product in products" :key="product.id">
        <Seminar :product="product" />
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

import Seminar from "@/components/Seminar.vue";
export default {
  name: "Seminar1",
  components: {
    Seminar,
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
      .get("http://localhost:3000/seminar")
      .then((response) => this.setProducts(response.data))
      .catch((error) => console.log(error));
  },
};
</script>

<style>
</style>