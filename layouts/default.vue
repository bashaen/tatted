<template>
  <div>
    <h1 class="title title--default">Tatted Up</h1>
    <nuxt/>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css?family=Aladin|Alex+Brush|Allura|Arizonia|Bilbo|Bilbo+Swash+Caps|Calligraffitti|Cookie|Dancing+Script|Kaushan+Script|Tangerine');

html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.title {
  background: rgba(0, 0, 0, .3);
  font-family: 'Dancing Script', cursive;
  font-weight: 800;
  font-size: 90px;
  margin: 0 auto;
  color: linen;
  letter-spacing: 1px;
  padding: 10px 25px;
  position: absolute;
  box-sizing: border-box;
  left: 0;
  right: 0;
  top: 100px;
  width: 100%;
  text-align: center;
}
input {
  outline: none;
  border: none;
  background: none;
  padding: 0;
}
.input--default {
  border: 1px solid #d3d3d3;
  display: block;
  margin: 10px auto;
  padding: 10px 5px;
  width: 90%;
}
input, button {
  outline: none;
}
</style>
