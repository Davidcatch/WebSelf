<template>
  <center>
    <div class="cards">
      <figure class="card">
        <figcaption class="card_title">
          <img
            width="50"
            height="50"
            src="https://img.icons8.com/color/48/vue-js.png"
            alt=""
          />
        </figcaption>
      </figure>
    </div>
  </center>
</template>

<script>
export default {
  name: 'About',
};
</script>

<style scoped>
.cards {
  perspective: 500px;
}

.card {
  width: 90px;
  height: 90px;
  position: relative;
  transform-style: preserve-3d;
  will-change: transform;
  transition: transform 0.5s;
}

.card:hover {
  transform: translateY rotateX(20deg) rotateY(20deg);
}

.card_title {
  color: #fff;
  position: absolute;
  top: 50%;
  right: 20px;
  transform: translateY(-50%);
  transition: transform 0.5s;
  font: 700 1.5rem monospace;
  text-shadow: -1px -1px 0 #000, 1px -1px 0 #000, -1px 1px 0 #000, 1px 1px 0 #000;
}

.card:hover .card_title {
  transform: translateZ(50px);
}
</style>
