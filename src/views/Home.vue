<template>
  <section id="home">
    <div class="container">
      <div class="flex flex-col mt-32 ml-16 absolute">
        <h2
          id="pos"
          class="text-3xl font-bold"
        >
          Front End Developer
        </h2>
        <h1 class="txt text-5xl flex gap-2">
          <b>Welcome To Home,</b>
          <p class="raihan font-semibold">Raihan.</p>
        </h1>
        <p class="w-96 text-xl leading-tight pt-2">
          Halo, Selamat Datang di Webself apa saja menu yang ada di webself ini yang pertama ada menu beranda yang isinya pengucapan selamat datang, yang kedua ada schedule atau jadwal matakuliah, yang ketiga ada todo list atau untuk
          mencatat tugas, yang keempat ada about atau tentang website ini.
        </p>
        <div class="logo flex gap-3 mt-10 ml-32">
          <div class="cards">
            <figure class="card">
              <figcaption class="card_title">
                <img
                  width="80"
                  height="80"
                  src="https://img.icons8.com/color/48/vue-js.png"
                  alt="vue-js"
                />
              </figcaption>
            </figure>
          </div>
          <div class="cards">
            <figure class="card">
              <figcaption class="card_title">
                <img
                  width="80"
                  height="80"
                  src="https://img.icons8.com/color/48/tailwindcss.png"
                  alt="tailwindcss"
                />
              </figcaption>
            </figure>
          </div>
          <div class="cards">
            <figure class="card">
              <figcaption class="card_title">
                <img
                  width="80"
                  height="80"
                  src="https://img.icons8.com/color/48/javascript--v1.png"
                  alt="javascript--v1"
                />
              </figcaption>
            </figure>
          </div>
        </div>
      </div>
      <div class="mt-24 right-10 absolute">
        <img
          src="../assets/img/photo4.png"
          alt=""
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Home',
};
</script>
