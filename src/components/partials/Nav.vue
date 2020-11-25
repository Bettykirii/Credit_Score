<template>

      <nav class="navbar">
        <div class="container">
        <div class="navbar-brand is-large">
          <a class="navbar-item" href="/">
      <strong class="is-size-4">CreditScore</strong>
    </a>

          <button @click="makeBurger" class="button navbar-burger" data-target="navMenu" v-bind:class="{ 'is-active': activator }">
              <span></span>
              <span></span>
              <span></span>
        </button>
        </div>
        <div class="navbar-menu" id="navMenu" v-bind:class="{ 'is-active': activator }">
          <div class="navbar-start">
      <router-link to="/" class="navbar-item">Home</router-link>
      <router-link to="/about" class="navbar-item">About</router-link>
      <router-link to="/profile" class="navbar-item">Profiles</router-link>
    </div>

      </div>
      </div>
    </nav>

</template>

<script>
export default {
  name: 'Navbar',
  data () {
    return {
      msg: '',
      activator: false
    }
  },
  methods: {
    makeBurger () {
      this.activator = !this.activator
      return this.activator
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
div{
  border: 0px solid black;
}
nav {
    margin-top: 25px;
    margin-bottom: 30px;
  
    a {
      font-weight: bold;
      text-align: center;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #d88d00;
      }
    }  
  } 

</style>