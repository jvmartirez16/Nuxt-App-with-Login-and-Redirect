<template>
  <div class="container">
    <nav>
      <div class="logo">
        <img src="/logo.png" alt="HIVEMED logo">
        <h2>HIVEMED</h2>
      </div>
      <ul>
        <li><NuxtLink to="/login">Login</NuxtLink></li>
        <li><NuxtLink to="/register">Register</NuxtLink></li>
      </ul>
    </nav>
    <div class="hero">
      <h1>Revolutionizing Healthcare</h1>
      <p>At HIVEMED, we're passionate about making healthcare more accessible, affordable, and efficient.</p>
      <NuxtLink to="/register" class="cta-button">Get Started</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  // ...
}
</script>

<style>
.container {
  max-width: 960px;
  margin: 0 auto;
  padding: 0 1rem;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 3rem;
  margin-top: 1rem;
}

.logo {
  display: flex;
  align-items: center;
}

.logo img {
  height: 2rem;
  margin-right: 0.5rem;
}

.logo h2 {
  font-size: 1.5rem;
  font-weight: bold;
}

ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

li {
  margin-right: 1rem;
}

a {
  text-decoration: none;
  color: #333;
}

.hero {
  margin-top: 2rem;
  text-align: center;
}

h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
  color: #0070f3;
}

p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: #444;
}

.cta-button {
  display: inline-block;
  background-color: #0070f3;
  color: white;
  border: none;
  border-radius: 4px;
  padding: 0.75rem 1.5rem;
  font-size: 1.2rem;
  text-decoration: none;
  cursor: pointer;
  transition: background-color 0.2s ease-in-out;
}

.cta-button:hover {
  background-color: #0060df;
}
</style>
