<template>
  <div class="dark-mode-toggle">
    <button @click="toggleDarkMode">
      <img
        v-if="isDarkMode"
        src="https://img.icons8.com/ios/50/sun--v1.png"
        alt="Light Mode"
        class=""
      />
      <img
        v-else
        src="https://img.icons8.com/ios-glyphs/30/bright-moon--v2.png"
        alt="Dark Mode"
      />
    </button>
  </div>
</template>

<script>
export default {
  name: 'DarkModeToggle',
  data() {
    return {
      isDarkMode: false,
    };
  },
  methods: {
    toggleDarkMode() {
      this.isDarkMode = !this.isDarkMode;
      document.body.classList.toggle('darkmode', this.isDarkMode);
    },
  },
  mounted() {
    // Check if dark mode is enabled on page load
    this.isDarkMode = localStorage.getItem('darkMode') === 'true';
    document.body.classList.toggle('darkmode', this.isDarkMode);
  },
  watch: {
    isDarkMode() {
      // Save dark mode state to local storage
      localStorage.setItem('darkMode', this.isDarkMode);
    },
  },
};
</script>

<style>
.dark-mode-toggle {
  position: absolute;
  top: 10px;
  right: 10px;
}

.dark-mode-toggle button {
  background-color: transparent;
  border: none;
  padding: 0;
}

.dark-mode-toggle img {
  width: 30px;
  height: 30px;
}
</style>
