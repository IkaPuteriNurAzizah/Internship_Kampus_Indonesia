<template>
  <section class="hero">
    <!-- Desktop -->
    <div class="d-none d-md-block">
      <div class="row mt-4">
        <div class="col-md-6">
          <div class="d-flex h-100">
            <div class="justify-content-center align-self-center">
              <h2>
                <strong>Bingung Cari Informasi Seputar Kuliah ?</strong>
              </h2>
              <h4>
                <strong>Cari Disini aja !</strong>
              </h4>
              <p>
                Dapatkan informasi seputar dunia perkuliahan secara terupdate
                dari kami melalui aplikasi Kampus Indonesia
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <img src="../assets/images/Hero.svg" />
        </div>
      </div>
      <div class="row mt-3 search_bar">
        <div class="col-md-8">
          <div class="input-group mb-3">
            <input
              v-model="search"
              type="text"
              class="form-control"
              placeholder="Informasi Seputar Perkuliahan/Cari Kampus"
              aria-label="Cari"
              aria-describedby="basic-addon1"
              @keyup="searchKampus"
            />
            <div class="input-group-prepend">
              <span class="input-group-text" id="basic-addon1">
                <b-icon-search></b-icon-search>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Mobile -->
    <div class="d-sm-block d-md-none">
      <div class="row mt-4">
        <div class="col-md-6 mb-3">
          <img src="../assets/images/Hero.svg" width="100%" />
        </div>
        <div class="col-md-6">
          <div class="d-flex h-100">
            <div class="justify-content-center align-self-center">
              <h2>
                <strong>Bingung Cari Informasi Seputar Kuliah ?</strong>
                <br />Cari Disini aja !
              </h2>
              <p>
                Dapatkan informasi seputar dunia perkuliahan secara terupdate
                dari kami melalui aplikasi Kampus Indonesia
              </p>
              <button class="btn btn-lg btn-success">
                <b-icon-arrow-right></b-icon-arrow-right>Pesan
              </button>
              <div class="row mt-3">
                <div class="col">
                  <div class="input-group mb-3">
                    <input
                      v-model="search"
                      type="text"
                      class="form-control"
                      placeholder="Cari Makanan Kesukaan Anda .."
                      aria-label="Cari"
                      aria-describedby="basic-addon1"
                      @keyup="searchKampus"
                    />

                    <div class="input-group-prepend">
                      <span class="input-group-text" id="basic-addon1">
                        <b-icon-search></b-icon-search>
                      </span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style>
</style>