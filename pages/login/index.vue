<template>
  <div class="login-page">
    <div class="form">
      <p v-if="errors.length">
      <ul>
        <li v-for="error in errors" v-bind:key="error">{{ error }}</li>
      </ul>
      </p>
      <form @submit.prevent="userLogin">
        <div>
          <label>Username</label>
          <input type="email" v-model="login.username" />
        </div>
        <div>
          <label>Password</label>
          <input type="password" v-model="login.password" />
        </div>
        <div>
          <button type="submit">Submit</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      login: {
        username: '',
        password: ''
      },
      errors: []
    }
  },
  methods: {
    async userLogin () {
      this.errors = []
      if (this.login.username && this.login.password) {
        try {
          const response = await this.$axios.$get('/login_user.json')
          console.log(response)
          if (
            this.login.username === response.username &&
            this.login.password === response.password
          ) {
            this.$store.commit('addToken', response.token)
            this.$router.push('/')
          } else {
            this.errors.push('Wrong username or password')
          }
        } catch (err) {
          console.log(err)
        }
      }

      if (!this.login.username) {
        this.errors.push('Username is required')
      }
      if (!this.login.password) {
        this.errors.push('Password is required')
      }
    }
  }
}
</script>

<style scoped>

.login-page {
  width: 360px;
  padding: 8% 0 0;
  margin: auto;
}

.form {
  position: relative;
  z-index: 1;
  background: #ffffff;
  max-width: 360px;
  margin: 0 auto 100px;
  padding: 45px;
  text-align: center;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24);
}

.form input {
  font-family: "Roboto", sans-serif;
  outline: 0;
  background: #f2f2f2;
  width: 100%;
  border: 0;
  margin: 0 0 15px;
  padding: 15px;
  box-sizing: border-box;
  font-size: 14px;
}

.form button {
  font-family: "Roboto", sans-serif;
  text-transform: uppercase;
  outline: 0;
  background: #4caf50;
  width: 100%;
  border: 0;
  padding: 15px;
  color: #ffffff;
  font-size: 14px;
  -webkit-transition: all 0.3 ease;
  transition: all 0.3 ease;
  cursor: pointer;
}

.form button:hover,
.form button:active,
.form button:focus {
  background: #43a047;
}

.form .message {
  margin: 15px 0 0;
  color: #b3b3b3;
  font-size: 12px;
}

body {
  background: #76b852; /* fallback for old browsers */
  background: -webkit-linear-gradient(right, #76b852, #8dc26f);
  background: -moz-linear-gradient(right, #76b852, #8dc26f);
  background: -o-linear-gradient(right, #76b852, #8dc26f);
  background: linear-gradient(to left, #76b852, #8dc26f);
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
