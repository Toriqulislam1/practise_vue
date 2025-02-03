<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <!-- Header / Navigation Bar -->
    <header class="navbar">
      <div class="logo">
        <h1>{{ msg }}</h1>
      </div>
      <nav class="nav-links">
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<style scoped>
/* Header/Navigation Bar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #2e3b4e;
  padding: 10px 20px;
  color: white;
}

.navbar .logo h1 {
  margin: 0;
  font-size: 1.8rem;
  font-weight: bold;
}

.navbar .nav-links ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.navbar .nav-links li {
  margin: 0 15px;
}

.navbar .nav-links a {
  color: white;
  text-decoration: none;
  font-size: 1.1rem;
  font-weight: 500;
}

.navbar .nav-links a:hover {
  color: #42b983; /* Green hover effect */
  text-decoration: underline;
}

.main-content {
  padding: 40px 20px;
  text-align: center;
}

@media (min-width: 1024px) {
  .navbar .nav-links ul {
    gap: 30px;
  }
}

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  .navbar .nav-links ul {
    flex-direction: column;
  }
}
</style>
