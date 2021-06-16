<template>
  <section class="artikel">
    <h3>
      <strong>Artikel Terbaru Kampus</strong>
    </h3>
    <p>Jangan sampai terlewat informasi terbaru kampus favoritmu</p>

    <b-carousel
      class="box"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide
        img-src="../assets/images/Artikel.svg"
        class="image_slide"
      >
        <b-badge class="badgee" pill variant="light">Artikel</b-badge>
        <h3 class="title">
          <strong>10 PTN Paling Diminati di SBMPTN 2020</strong>
        </h3>
        <p class="desc">14 September 2020</p>
      </b-carousel-slide>

      <b-carousel-slide
        img-src="../assets/images/Artikel.svg"
        class="image_slide"
      >
        <b-badge class="badgee" pill variant="light">Artikel</b-badge>
        <h3 class="title">
          <strong>10 PTN Paling Diminati di SBMPTN 2020</strong>
        </h3>
        <p class="desc">14 September 2020</p>
      </b-carousel-slide>

      <b-carousel-slide
        img-src="../assets/images/Artikel.svg"
        class="image_slide"
      >
        <b-badge class="badgee" pill variant="light">Artikel</b-badge>
        <h3 class="title">
          <strong>10 PTN Paling Diminati di SBMPTN 2020</strong>
        </h3>
        <p class="desc">14 September 2020</p>
      </b-carousel-slide>
    </b-carousel>
  </section>
</template>

<script>
export default {
  name: "Artikel",
};
</script>

<style>
</style>