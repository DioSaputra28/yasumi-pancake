<script setup>
</script>

<template>
  <div id="app-container">
    <header class="header">
      <button class="menu-button">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <line x1="3" y1="12" x2="21" y2="12"></line>
          <line x1="3" y1="6" x2="21" y2="6"></line>
          <line x1="3" y1="18" x2="21" y2="18"></line>
        </svg>
      </button>
    </header>
    <main class="main-content">
      <div class="content-wrapper">
        <div class="title-section">
          <h1>YASUMI.</h1>
          <h2>PANCAKE</h2>
        </div>
        <p class="description">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt dui ac odio euismod, eu porta odio euismod. Maecenas consectetur lorem a blandit porta.
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt dui ac odio euismod, eu porta odio euismod.
        </p>
        <nav class="main-nav">
          <a href="#" class="nav-button">MENU</a>
          <a href="#" class="nav-button">ABOUT US</a>
          <a href="#" class="nav-button">CONTACT</a>
        </nav>
      </div>
      <div class="image-section">
        <img src="@/assets/pancake.jpg" alt="Pancake" class="pancake-image">
        <p class="description">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt dui ac odio euismod, eu porta odio euismod. Maecenas consectetur lorem a blandit porta.
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt dui ac odio euismod, eu porta odio euismod.
        </p>
      </div>
    </main>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Anton&family=Roboto:wght@400;700&display=swap');

#app-container {
  background-color: #FCECDD;
  min-height: 100vh;
  font-family: 'Roboto', sans-serif;
}

.header {
  background: url('@/assets/kitchen-background.jpg') no-repeat center center;
  background-size: cover;
  height: 200px;
  position: relative;
}

.menu-button {
  position: absolute;
  top: 20px;
  right: 20px;
  background: transparent;
  border: none;
  cursor: pointer;
}

.menu-button svg {
  stroke: white;
  width: 30px;
  height: 30px;
}

.main-content {
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.title-section h1 {
  font-family: 'Anton', sans-serif;
  font-size: 4rem;
  color: #B5482A;
  margin: 0;
  line-height: 1;
}

.title-section h2 {
  font-family: 'Anton', sans-serif;
  font-size: 2.5rem;
  color: #B5482A;
  margin: 0;
  line-height: 1;
}

.description {
  color: #333;
  line-height: 1.6;
  margin: 20px 0;
}

.main-nav {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-top: 20px;
}

.nav-button {
  padding: 15px;
  color: white;
  text-align: center;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.2rem;
  border: none;
}

.nav-button:nth-child(1) {
  background-color: #EC7C35;
}

.nav-button:nth-child(2) {
  background-color: #707954;
}

.nav-button:nth-child(3) {
  background-color: #B48A6D;
}

.pancake-image {
  width: 100%;
  max-width: 400px;
  display: block;
  margin: 0 auto 20px;
  border-radius: 8px;
}

/* Responsive styles */
@media (min-width: 768px) {
  .main-content {
    flex-direction: row;
    align-items: flex-start;
    padding: 40px;
  }

  .content-wrapper {
    flex: 1;
    padding-right: 40px;
  }

  .image-section {
    flex: 1;
  }

  .pancake-image {
    margin: 0 0 20px;
  }
}
</style>