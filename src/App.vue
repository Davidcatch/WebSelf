<template>
  <div>
    <header
      ref="header"
      class="p-4"
    >
      <div class="container mx-auto flex justify-between">
        <img
          src="./assets/img/Logo2.png"
          alt="#"
          class="w-20 ml-16"
        />
        <nav class="mr-40">
          <ul class="flex space-x-4">
            <li>
              <router-link
                to="/"
                class="hover:text-gray-400"
                >Home</router-link
              >
            </li>
            <li>
              <router-link
                to="/schedule"
                class="hover:text-gray-400"
                >Schedule</router-link
              >
            </li>
            <li>
              <router-link
                to="/todo"
                class="hover:text-gray-400"
                >To-Do List</router-link
              >
            </li>
            <li>
              <router-link
                to="/about"
                class="hover:text-gray-400"
                >About</router-link
              >
            </li>
          </ul>
        </nav>
      </div>
    </header>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'app',
  mounted() {
    // Set the background color when the component is mounted
    document.body.style.backgroundColor = '#F1F0E8';

    // Access the <nav> element using $refs and set its background color
    this.$refs.header.style.backgroundColor = '#e5e1da';
    this.$refs.header.style.color = 'black'; // Optional: Change text color
  },
};
</script>
