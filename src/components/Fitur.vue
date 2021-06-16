<template>
  <section class="fitur">
    <h3>
      <strong>Fitur yang Tersedia di Kampus Indonesia</strong>
    </h3>
    <div class="box">
      <b-card-group deck>
        <b-card
          class="box_card shadow"
          img-src="../assets/images/Fitur/Kampus.svg"
          img-alt="Image"
          img-top
        >
          <b-card-text class="card_title">Kampus</b-card-text>
        </b-card>

        <b-card
          class="box_card shadow"
          img-src="../assets/images/Fitur/Beasiswa.svg"
          img-alt="Image"
          img-top
        >
          <b-card-text class="card_title">Beasiswa</b-card-text>
        </b-card>

        <b-card
          class="box_card shadow"
          img-src="../assets/images/Fitur/Workshop.svg"
          img-alt="Image"
          img-top
        >
          <b-card-text class="card_title">Workshop</b-card-text>
        </b-card>
      </b-card-group>

      <b-card-group deck>
        <b-card
          class="box_card shadow"
          img-src="../assets/images/Fitur/Lomba.svg"
          img-alt="Image"
          img-top
        >
          <b-card-text class="card_title">Lomba</b-card-text>
        </b-card>

        <b-card
          class="box_card shadow"
          img-src="../assets/images/Fitur/Lowongan.svg"
          img-alt="Image"
          img-top
        >
          <b-card-text class="card_title">Lowongan</b-card-text>
        </b-card>

        <b-card
          class="box_card shadow"
          img-src="../assets/images/Fitur/UTBK.svg"
          img-alt="Image"
          img-top
        >
          <b-card-text class="card_title">UTBK</b-card-text>
        </b-card>
      </b-card-group>
    </div>
  </section>
</template>

<script>
export default {
  name: "Fitur",
};
</script>

<style>
</style>