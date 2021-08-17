<template>
<div id="App">
  <main>
    <div class="search-box">
      <input type="text" class="search-bar" placeholder="Search..." />
    </div>
  </main>
</div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      api_key: 'd4aefba1b367102b2faac27255f9fa3d'
      }
}
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  }

  body{
    font-family: 'montserrat', sans-serif;
    }

  #App{
    background-image: url('./assets/weatherFW.jpg');
    background-size: cover;
    background-position: bottom;
    transition: 0.5s;
    }

  main{
    min-height: 100vh;
    padding: 25px;
    background-image: linear-gradient(to bottom, rgba(0,0,0,0.25), rgba(0,0,0,0.75) );
    }

  .search-box{
    width: 100%;
    margin-bottom: 30px;
    }

    .search-box .search-bar{
      display: block;
      width: 100%;
      padding: 10px;
      color: black;
      font-size: 25px;
      appearance: none;
      border: none;
      outline: none;
      background: none;
      background-color: rgb(255, 255, 255, 0.5);
      border-radius: 5px 16px 10px 27px;

    }
</style>8