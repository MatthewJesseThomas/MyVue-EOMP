<template>
    <form id="registerForm" @submit="handleSubmit">
      <h2>New Account</h2>
      <div class="inputBox">
        <input v-model="username" type="text" required>
        <label>Username</label>
      </div>
      <div class="inputBox">
        <input v-model="email" type="text" required>
        <label>Email</label>
      </div>
      <div class="inputBox">
        <input v-model="password" type="password" required>
        <label>Create &nbsp; Password</label>
      </div>
      <div class="inputBox">
        <input v-model="confirmPassword" type="password" required>
        <label>Confirm &nbsp; Password</label>
      </div>
      <div class="inputBox">
        <input type="submit" value="Create">
      </div>
      <p>Already Have an Account!!! <a href="./pages/login.html">Login</a></p>
    </form>
  </template>
  
  <script>
  import Swal from 'sweetalert2';
  
  export default {
    data() {
      return {
        username: '',
        email: '',
        password: '',
        confirmPassword: '',
      };
    },
    methods: {
      handleSubmit(event) {
        event.preventDefault();
        const { username, email, password, confirmPassword } = this;
        const values = { username, email, password, confirmPassword };
        console.log(values);
  
        Swal.fire({
          title: 'Congrats',
          text: 'Data Successfully Logged',
          icon: 'success',
          confirmButtonText: 'OK',
        });
      },
    },
  };
  </script>

  <style lang="css" scoped>
  @import url('https://fonts.googleapis.com/css?family=Poppins:200,300,400,500,600,700,800,900&display=swap');
  
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
  }
  
  :root {
    --clr: crimson;
  }
  
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #1c2630;
  }
  
  form {
    background: #29313c;
    padding: 60px 80px 60px;
    text-align: center;
    display: flex;
    flex-direction: column;
    border-radius: 12px;
    max-width: 400px; /* Added to limit the form width */
    width: 100%; /* Added to make the form responsive */
  }
  
  form h2 {
    color: #fff;
    font-weight: 500;
    text-transform: uppercase;
    font-size: 1.3rem;
    letter-spacing: 0.1em;
    margin-bottom: 50px;
  }
  
  .inputBox {
    position: relative;
    width: 100%;
    margin-bottom: 40px;
  }
  
  .inputBox input {
    position: relative;
    width: 100%;
    padding: 1px 0;
    background: none;
    border-bottom: 3px solid #999;
    outline: none;
    color: #cdf2ff;
    font-size: 1em;
    text-transform: capitalize;
    letter-spacing: 0.23em;
  }
  
  .inputBox label {
    position: absolute;
    left: 0;
    padding: 10px 0;
    pointer-events: none;
    color: #999;
    text-transform: uppercase;
  }
  
  .inputBox label span {
    position: relative;
    display: inline-flex;
    letter-spacing: 0.05em;
    transition: 0.2s ease-in-out;
  }
  
  .inputBox input:focus ~ label span,
  .inputBox input:valid ~ label span {
    color: var(--clr);
    letter-spacing: 0.15em;
    transform: translateY(-25px);
  }
  
  .inputBox input:focus,
  .inputBox input:valid {
    border-bottom: 2px solid var(--clr);
  }
  
  .inputBox input[type="submit"] {
    background: var(--clr);
    border: none;
    padding: 15px;
    border-radius: 50px;
    color: #1c2630;
    font-weight: 600;
    font-size: 1.15em;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    cursor: pointer;
    transition: 0.5s;
  }
  
  .inputBox input[type="submit"]:hover {
    letter-spacing: 0.35em;
    scale: 1.05;
  }
  
  form p {
    color: #fff;
    font-size: 0.9em;
    margin-bottom: 40px;
  }
  
  form p a {
    color: var(--clr);
    font-weight: 600;
    text-decoration: none;
  }
  </style>