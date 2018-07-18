<template>
  <div class="container home-container">
    <div>
      <img src="./assets/logo.png">
      <h1>{{ msg }}</h1>
    </div>

    <div class="row">
      <div class="col-12 col-md-6">
        <button type="button" name="button" class="btn btn-primary">
          Primary-colored Button
        </button>
      </div>
      <div class="col-12 col-md-6">
        <button type="button" name="button" class="btn btn-secondary">
          Secondary-colored Button
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">
$primary: #d21034;
$secondary: #ddd;

.home-container {
  font-family: 'Roboto', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

// Note: for some reason imported Bootstrap sass file should be at the end of style scripts :X

@import '../node_modules/bootstrap/scss/bootstrap.scss';
</style>
