<template>
  <section class="container">
    <video class='flexible' autoplay="" name="media" muted>
      <source src="/video/ass.mp4" type="video/mp4">
    </video>
    <div class="video-overlay"></div>
    <nuxt-link to="/register" class="registration-button">Sign Up or Log In</nuxt-link>
  </section>
</template>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.registration-button {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, .3);
  /* background: transparent; */
  border: none;
  border-top: 3px solid linen;
  outline: none;
  height: 75px;
  color: linen;
  font-size: 34px;
  text-decoration: none;

  /* font-family: "Aladin"; */
  /* font-family: "Allura"; */
  /* font-family: "Bilbo"; */
  /* font-family: "Bilbo Swash Caps"; */
  /* font-family: "Calligraffitti"; */
  font-family: "Cookie";
  /* font-family: "Kaushan Script"; */
  /* font-family: "Tangerine"; */
  font-weight: bold;
  padding-bottom: 35px;
}

.registration-button:after {
  content: "";
  display: block;
  width: 25px;
  height: 25px;
  border-right: 5px solid linen;
  border-bottom: 5px solid linen;
  margin: 0 auto;
  margin-top: -8px;
  transform: rotate(45deg);
  -webkit-transform: rotate(45deg);
  position: relative;

  animation-name: bounce;
  animation-duration: 3s;
  animation-iteration-count: infinite;
}

@keyframes bounce {
  0%   {top: 0px;}
  10%  {top: 8px;}
  17%  {top: 4px;}
  27%  {top: 8px;}
  34%  {top: 0px;}
}

.flexible { 
  /* position:absolute;
  object-fit: cover;
  width: 100%;
  height: 100%; */

  position: fixed;
  top: 50%;
  left: 50%;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  z-index: -100;
  transform: translate(-50%, -50%);
}

.video-overlay {
  /* background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAICAYAAADED76LAAAAQElEQVQYlW2OwQ0AMAgCbw7XcMFubj81RVpeGgIcQHK1gJC/+shjtkLNTmpTaZMm05IB76YzfTedaW46k28Opg1VYQ5hW3JdzwAAAABJRU5ErkJggg==) repeat; */
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAIElEQVQYV2NctmzZ/6ioKEZkmpGBgYEBXQJFBUwH8SoB8vAw2drpptMAAAAASUVORK5CYII=) repeat;
  position: fixed;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  top: 0;
  left: 0;
  z-index: -100;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

input {
  outline: none;
}
</style>
