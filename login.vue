<template>
    <div>
      <!-- Conditionally render content based on authentication state -->
      <div v-if="isAuthenticated">
        <h2>You are in!</h2>
        <button @click="logout">Logout</button>
      </div>
      <div v-else-if="isLoggingIn">
        <p>loading</p>
      </div>
      <div v-else>
        <h2>Login</h2>
        <input v-model="usernameInput" placeholder="Username" />
        <input v-model="passwordInput" type="password" placeholder="Password" />
        <button @click="login">Login</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isAuthenticated: false,
        isLoggingIn: false,
        usernameInput: '',
        passwordInput: '',
      };
    },
    methods: {
      login() {
        // Simulate a login request (replace with actual authentication logic)
        this.isLoggingIn = true;
        setTimeout(() => {
          if (this.usernameInput === 'Labiba' && this.passwordInput === 'labiba123') {
            this.isAuthenticated = true;
          } else {
            alert('Invalid credentials. Please try again.');
          }
          this.isLoggingIn = false;
        }, 3000);
      },
      logout() {
        this.isAuthenticated = false;
        this.usernameInput = '';
        this.passwordInput = '';
      },
    },
  };
  

  </script>
  