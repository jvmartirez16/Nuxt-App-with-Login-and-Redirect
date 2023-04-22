<template>
    <div>
      <nav>
        <ul>
          <li><a href="/">Home</a></li>
          <li @click.prevent="logout"><a href="#">Logout</a></li>
        </ul>
      </nav>
      <div class="container">
        <h1>Dashboard</h1>
        <p>Welcome to your dashboard, {{ username }}!</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        username: '' // replace with actual username
      }
    },
    methods: {
      logout() {
        // TODO: Implement logout logic
        console.log('Logged out');
        window.location.href = '/';
      }
    }
  }
  </script>
  
  <style>
    nav {
      background-color: #0070f3;
      color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem;
    }
  
    ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      display: flex;
      align-items: center;
    }
  
    li {
      margin-left: 1rem;
    }
  
    li:first-child {
      margin-left: 0;
    }
  
    li a {
      color: white;
      text-decoration: none;
    }
  
    li a:hover {
      text-decoration: underline;
    }
  
    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 0 1rem;
      text-align: center;
    }
  
    h1 {
      margin-top: 2rem;
    }
  
    p {
      margin-top: 1rem;
      font-size: 1.2rem;
    }
  </style>
  