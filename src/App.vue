<template>
  <header>
    <h1>Image Gallery</h1>
  </header>
  <router-view :imgData="imgData"/>
</template>

<script>
import imageData from './imageData.json'


export default {
  data() {
    return{
      imgData: imageData
    }
  },
}
</script>

<style>
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body{
    background: khaki;
  }

  header{
    background: lightcoral;
    height: 10vh;
    width: 100%;
    margin-bottom: 1rem;
  }

  h1{
    font-size: 2rem;
    text-align: center;
    position: relative;
    top:25%;
    letter-spacing: 2px;
    color: wheat;
  }

  h2{
    text-align: center;
    color: lightcoral;
  }

  .imageContainer,
  img{
    display: block;
    width: 50%;
    margin: 5% auto;
  }

  img{
    padding: 10%;
    margin: 0 auto;
  }


  .name{
    text-align: center;
    font-size: 1.5rem;
    color: lightgray;
    text-shadow: 1px 1px #111;

}
</style>
