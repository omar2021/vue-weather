<template>
<div id="App">
  <main>
    <div class="search-box">
      <input type="text" class="search-bar" placeholder="Search..." />
    </div>

    <div class="weather-wrap">
      <div class="location-box">
        <div class="location">
          Irvine, US
        </div>
        <div class="date">
          Tuesday 20 May 2020
        </div>
      </div>
      <div class="weather-box">
        <div class="temp">81 F</div>
        <div class="weather">Sunny</div>
      </div>
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
    /* Photo by noaa-99f4 - Unsplash  */
  
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
      box-shadow: 0px 0px 8px rgba(0,0,0,0.25);
      background-color: rgb(255, 255, 255, 0.5);
      border-radius: 5px 16px 10px 27px;
      transition: 00.5s;
    }

    .search-box .search-bar:focus {
      box-shadow: 0px 0px 16px rgba(0,0,0,0.25);
      background-color: rgb(255, 255, 255, 0.5);
      border-radius: 16px 0px 16px 0px;
    }

    .location-box .location {
        color: #ffD;
        font-size: 34px;
        font-weight: 500;
        text-align: center;
        text-shadow: rgba(0,0,0,0.25);
    }

    .location-box .date {
      color: #ffD;
      font-size: 22px;
      font-weight: 400;
      font-style: italic;
      text-align: center;
    }


</style>