<template>
  <section class="kampus">
    <b-card-group deck>
      <b-card class="box_card shadow">
        <div class="latar">
          <img :src="'assets/images/' + product.gambar" alt="Image" img-top />
        </div>

        <div class="logo">
          <img :src="'assets/images/' + product.logo" alt="..." />
        </div>

        <div class="card_body">
          <h5 class="card_title">
            <strong>{{ product.nama }}</strong>
          </h5>
          <h7 class="card_text">
            Akreditasi : {{ product.akreditasi }} <br /><br
          /></h7>
          <router-link class="btn btn-primary" :to="'/list1/' + product.id"
            ><b-icon-book></b-icon-book> Lihat Detail</router-link
          >
        </div>
      </b-card>
    </b-card-group>
  </section>
</template>

<script>
export default {
  name: "Kampus",
  props: ["product"],
};
</script>

<style>
</style>