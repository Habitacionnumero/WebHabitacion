<template>
<div class="main">
      <div class="main_top">
        <div class="main_top_title">
          <router-link :to="{ name: 'home' }"
            ><img  src="/img/titulo2.png" alt=""
          /></router-link>


        </div>
      <marquee>
        <a href="https://rgbshop38191613162016135.com/" target = "_blank" class="banner"> <img class="avion_img" src="/img/banner.png" alt=""></a>
      </marquee>
      <div class="main_top_menu">
        <div class="main_top_doors max-width">
          <router-link :to="{ name: 'instalaciones' }" 
            ><img class="install_door" src="/img/puerta_origin.png"  alt=""
          /></router-link>
          
          <a href="https://rgbshop38191613162016135.com" target = "_blank">
              <img class="rgb_door" src="/img/puerta_rgb.png" alt="">
          </a>

          <router-link :to="{ name: 'meta' }" 
            ><img class="meta_door" src="/img/puerta_future.png" alt=""
          /></router-link>

          <router-link :to="{ name: 'instalaciones' }" class="pc"
            ><img class="install_door" src="/img/puerta_origin.png"  alt=""
          /></router-link>

          <a href="https://rgbshop38191613162016135.com/" target = "_blank" class="pc">
              <img class="rgb_door" src="/img/puerta_rgb.png" alt="">
          </a>

          <router-link :to="{ name: 'meta' }" class="pc"
            ><img class="meta_door" src="/img/puerta_future.png" alt=""
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


.main_top {
  min-height: 85vh;
  background: url("/img/fondo_junto.png");
  background-size: cover;
  background-position: right 65% bottom 65% ;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  //gap: 1em;
  padding-top: 10em;

}
.main_top_menu{
  margin-right: 300px;
}

.main_top_title{
  margin-top: -1em;
  //max-width: $mx-tablet-grande;
  max-width: 684px;
}
.main_top_doors {
  //justify-content: center;
  padding-top: 1em;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr ;
}
.main_bottom_content {
  background: url("/img/suelo.png");
  background-size: cover;
  display: flex;
  justify-content: center;
  height: 280px;
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
 right: 14em;
 width: 300px;
}
.contacto {
  transform: rotate(15deg);
  top: -3em;
  width: 300px;
  left:8em;
}
.prensa {
  transform: rotate(-10deg);
  top: -3em;
  left: 29em;
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
  width: 500px;
}
.avion_img{
  padding-top: 0em;
  width: 500px;
  min-width: 100px;
  margin-left: 0px;
}

.meta_door, .install_door, .rgb_door{
  padding: 10px;
  width: 280px;

}

.pc{
  display: none;
}





@media screen  and (max-width: 800px) {

.main_top_title {
  margin-top:-58px;
}
.main_top_menu {
  overflow: hidden;
  width: 100%;
  height: 400px;  
  margin-right: 0px;

}

.avion_img {
margin-top: 20px;
width: 500px;
min-width: 100px;
}

.aplica {
margin-top: 2.5em;
right: -4em;
max-width: 100px;
}
.contacto {
margin-top: 2.5em;
max-width: 100px;
left: 1em;
}
.prensa {
margin-top: 2.5em;
left:1em;
max-width: 100px;
}

.tarjeta {
max-width: 50px;
}
.main_bottom_content {
height: 150px;
}
.pc{
display: inline;
}
.main_top_doors {
animation: scroll 10s linear infinite;
grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
margin-top: -10px;
}

.meta_door, .install_door, .rgb_door{
width: 163px;
padding: 0px;
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
