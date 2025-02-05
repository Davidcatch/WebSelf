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
        <h1 class="text-5xl"><b>Welcome To Home,</b> Raihan.</h1>
        <p class="w-96 text-xl leading-tight pt-2">Lorem ipsum dolor sit amet consectetur. Dapibus dictumst dignissim gravida turpis lacus id amet turpis. Aliquam diam dignissim est fringilla scelerisque tellus pharetra mauris.</p>
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
