<template>
  <section
    id="schedule"
    class="mt-10"
  >
    <div class="judul text-center">
      <h1 class="text-3xl font-bold">Jadwal Mata Kuliah Semester 3</h1>
    </div>
    <div class="jadwal inline-grid grid-cols-3 gap-10 text-sm leading-6 mt-10 ml-20">
      <div class="senin">
        <h1 id="senin">
          <u class="text-2xl"><b>Senin</b></u>
        </h1>
        <div class="flex gap-5">
          <p>08:30 - 10:30</p>
          <p>Proyek Tingkat II | R</p>
        </div>
        <p class="text-center">D</p>
      </div>
      <div class="selasa">
        <h1 id="selasa">
          <u class="text-2xl"><b>Selasa</b></u>
        </h1>
        <div class="flex gap-5">
          <p>07:30 - 10:30</p>
          <p>Basis Data | R</p>
        </div>
        <p class="text-center">D</p>
        <div class="flex gap-5">
          <p>10:30 - 13:30</p>
          <p>Arsitektur Dan Desain Perangkat Lunak | R</p>
        </div>
        <p class="text-center">D</p>
        <div class="flex gap-5">
          <p>12:30 - 15:30</p>
          <p>Konstruksi Perangkat Lunak | R</p>
        </div>
        <p class="text-center">D</p>
      </div>
      <div class="Rabu">
        <h1 id="rabu">
          <u class="text-2xl"><b>Rabu</b></u>
        </h1>
        <div class="flex gap-5">
          <p>07:30 - 10:30</p>
          <p>Arsitektur Dan Desain Perangkat Lunak | R</p>
        </div>
        <p class="text-center">D</p>
        <div class="flex gap-5">
          <p>10:30 - 13:30</p>
          <p>Rekayasa Kebutuhan Perangkat Lunak | R</p>
        </div>
        <p class="text-center">D</p>
        <div class="flex gap-5">
          <p>13:30 - 16:30</p>
          <p>Konstruksi Perangkat Lunak | R</p>
        </div>
        <p class="text-center">D</p>
      </div>
      <div class="Kamis">
        <h1 id="kamis">
          <u class="text-2xl"><b>Kamis</b></u>
        </h1>
        <div class="flex gap-5">
          <p>10:30 - 13:30</p>
          <p>Basis Data | R</p>
        </div>
        <p class="text-center">D</p>
        <div class="flex gap-5">
          <p>13:30 - 16:30</p>
          <p>Interaksi Manusia Komputer | R</p>
        </div>
        <p class="text-center">D</p>
      </div>
      <div class="Jumat">
        <h1 id="jumat">
          <u class="text-2xl"><b>Jumat</b></u>
        </h1>
        <div class="flex gap-5">
          <p>08:30 - 11:30</p>
          <p>Pemodelan Perangkat Lunak | R</p>
        </div>
        <p class="text-center">D</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Schedule',
};
</script>
