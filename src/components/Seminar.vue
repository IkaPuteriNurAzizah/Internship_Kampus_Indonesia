<template>
  <section class="seminar">
    <b-card-group deck>
      <b-card class="box_card shadow">
        <div class="latar">
          <img :src="'assets/images/' + product.gambar" alt="..." />
        </div>

        <div class="card_body">
          <h5 class="card-title">
            <strong>{{ product.nama }}</strong>
          </h5>
          <h7 class="card_text">
            Tanggal : {{ product.tanggal }} <br />Via : {{ product.via
            }}<br /><br />
          </h7>
          <router-link class="btn btn-primary" :to="'/info/' + product.id"
            ><b-icon-book></b-icon-book> Lihat Detail</router-link
          >
        </div>
      </b-card>
    </b-card-group>
  </section>
</template>

<script>
export default {
  name: "Seminar",
  props: ["product"],
};
</script>

<style>
</style>