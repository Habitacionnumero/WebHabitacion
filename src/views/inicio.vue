<template>
<div class="main">
      <div class="main_top">
        <div class="main_top_title">
          <router-link :to="{ name: 'home' }"
            ><img  src="/img/titulo2.png" alt=""
          /></router-link>
      </div>
          <marquee class="fly">
          <a href="https://rgbshop38191613162016135.com/" target = "_blank"> <img class="avion_img" src="/img/avionetaGif2.gif" alt=""></a>
          </marquee>
      <div class="main_top_menu">
        <div class="main_top_doors max-width">
          <router-link :to="{ name: 'instalaciones' }" 
            ><img class="install_door" src="/img/originNeon.png"  alt=""
          /></router-link>
          
          <a href="https://rgbshop38191613162016135.com" target = "_blank">
              <img class="rgb_door" src="/img/rgbNeon.png" alt="">
          </a>

          <router-link :to="{ name: 'meta' }" 
            ><img class="meta_door" src="/img/futureNeon.png" alt=""
          /></router-link>

          <router-link :to="{ name: 'instalaciones' }" class="pc"
            ><img class="install_door" src="/img/originNeon.png"  alt=""
          /></router-link>

          <a href="https://rgbshop38191613162016135.com/" target = "_blank" class="pc">
              <img class="rgb_door" src="/img/rgbNeon.png" alt="">
          </a>

          <router-link :to="{ name: 'meta' }" class="pc"
            ><img class="meta_door" src="/img/futureNeon.png" alt=""
          /></router-link>
         
          <!-- <router-link :to="{ name: 'residencias' }"
            ><img src="/img/puerta_residencias.png" alt=""
          /></router-link> -->
        </div>
      </div>
    </div>
    <div class="main_bottom_content">
      <div class="main_bottom">
        <router-link :to="{ name: 'about' }"
          ><div class="tarjeta">
            <img src="/img/tarjeta_aplica.png" alt="" class="aplica" /></div
        ></router-link>
        <router-link :to="{ name: 'contacto' }"
          ><div class="tarjeta">
            <img src="/img/tarjeta_contacto.png" alt="" class="contacto" /></div
        ></router-link>

        <router-link :to="{ name: 'prensa' }"
          ><div class="tarjeta">
            <img src="/img/tarjeta_prensa.png" alt="" class="prensa" /></div
        ></router-link>
      </div>
    </div>
  </div>
</template>



<style lang="scss" scoped>

.fly{
  width: 100%;
}
.main_top {
  min-height: 88vh;
  background: url("/img/fondo_junto_noche3.png");
  background-size: cover;
  background-position: right 65% bottom 55% ;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  //gap: 1em;
  padding-top: 0em;

}
.main_top_menu{
  margin-right: 300px;
}

.main_top_title{
  margin-top: 1.1em;
  //max-width: $mx-tablet-grande;
  max-width: 835px;
}
.main_top_doors {
  //justify-content: center;
  padding-top: 4.0em;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr ;
}
.main_bottom_content {
  background: url("/img/suelo.png");
  background-size: cover;
  display: flex;
  justify-content: center;
  height: 235px;
  margin-top: -48px;
}
.main_bottom{
  display: grid;
  grid-template-columns: 2.5fr 2.5fr 2.5fr ;
  //padding: 25px;
  max-width: $mx-tablet;
  min-width: 390px;
}
.aplica {
 transform: rotate(-15deg);
 position: absolute;
 top: -3em;
 right: 10em;
 width: 300px;
}
.contacto {
  transform: rotate(15deg);
  top: -3em;
  width: 300px;
  left: 8em;
}
.prensa {
  transform: rotate(-10deg);
  top: -3em;
  left: 25em;
  width: 300px;
}
.anuncio{
  //width: 50%;
  margin-bottom: 50px;
  display: grid;
  grid-template-columns:4fr 12fr;
  //margin-right: 0px;
}

.banner{
  width: 650px;
}
.avion_img{
  padding-top: 30px;
  height: 180px;
  width: 750px;
  min-width: 100px;
  margin-left: 0px;
}
.meta_door, .install_door, .rgb_door{
  padding: 10px;
  width: 240px;
}


.pc{
  display: none;
}





@media screen  and (max-width: 800px) {

.main_top_title {
  margin-top:10px;
  width: 380px;
}
.main_top {
  min-height: 95vh;
  background: url("/img/fondo_junto_noche3.png");
  background-size: cover;
  background-position: right 65% bottom 65% ;
}
.main_top_menu {
  overflow: hidden;
  width: 100%;
  height: 480px;  
  margin-top: -40px;
  margin-right: 0px;
}

.avion_img {
margin-top: -50px;
width: 500px;
min-width: 100px;
}

.aplica {
margin-top: 2.1em;
right: -4.7em;
max-width: 113px;
}
.contacto {
margin-top: 2.1em;
max-width: 113px;
left: 1em;
}
.prensa {
margin-top: 2.1em;
left: 0.7em;
max-width: 113px;
}

.tarjeta {
max-width: 50px;
}
.main_bottom_content {
height: 150px;
margin-top: -67px;
}
.pc{
display: inline;
}
.main_top_doors {
animation: scroll 10s linear infinite;
grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
margin-top: -2px;
}

.meta_door, .install_door, .rgb_door{
width: 174px;
padding-top: -50px;
}
@keyframes scroll {
0%{
  transform: translateX(0);
}
  100%{
    transform: translateX(calc(-163px * 3));
  }
}
}
</style>
