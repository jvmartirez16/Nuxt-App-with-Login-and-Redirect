<template>
    <div class="container">
      <h1>Register</h1>
      <form @submit.prevent="signup">
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" required>
  
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" required>
  
        <label for="password">Password:</label>
        <input type="password" id="password" v-model="password" required>
  
        <button type="submit">Signup</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        email: '',
        password: ''
      }
    },
    methods: {
      signup() {
        // TODO: Implement signup logic
        console.log('Signed up with name:', this.name, ' email:', this.email, ' password:', this.password);
      }
    }
  }
  </script>
  
  <style>
    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 0 1rem;
      text-align: center;
    }
  
    h1 {
      margin-top: 2rem;
    }
  
    form {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 2rem;
    }
  
    label {
      display: block;
      margin-bottom: 0.5rem;
      font-weight: bold;
    }
  
    input[type="text"],
    input[type="email"],
    input[type="password"] {
      width: 100%;
      padding: 0.5rem;
      margin-bottom: 1rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 1rem;
    }
  
    button[type="submit"] {
      background-color: #0070f3;
      color: white;
      border: none;
      border-radius: 4px;
      padding: 0.5rem 1rem;
      font-size: 1rem;
      cursor: pointer;
    }
  </style>
  