<script setup>
import MenuNavegacion from "../components/MenuNavegacion.vue";
</script>
<template>
  <div class="prensa_main">
    <div class="prensa_content">
      <div class="prensa_enlaces">
        <a target="_blank" href="https://www.instagram.com/luciarojo__/"
          ><img src="/img/lenadelucia.webp" alt=""
        /></a>
        <a target="_blank" href="https://www.instagram.com/hell0javi/"
          ><img src="/img/javi_martin.webp" alt=""
        /></a>
        <a target="_blank" href="https://www.instagram.com/i0o0.0o0.i/"
          ><img src="/img/carlos_rubio.webp" alt=""
        /></a>
      </div>
      <div class="prensa_enlaces">
        <a
          target="_blank"
          href="https://www.instagram.com/lorenzogalgo/?igshid=YmMyMTA2M2Y%3D"
          ><img src="/img/lorenzo_galgo.webp" alt=""
        /></a>
        <a
          target="_blank"
          href="https://www.instagram.com/mash_kb/?igshid=YmMyMTA2M2Y%3D"
          ><img src="/img/masaaki.webp" alt=""
        /></a>
        <a
          target="_blank"
          href="https://www.instagram.com/enriqueyanezsalgado/?igshid=YmMyMTA2M2Y%3D"
          ><img src="/img/enrique.webp" alt=""
        /></a>
      </div>
      <div class="prensa_enlaces">
        <a
          target="_blank"
          href="https://www.instagram.com/alejandria.cinque/?igshid=YmMyMTA2M2Y%3D"
          ><img src="/img/alejandria.webp" alt=""
        /></a>
        <div>
          <img src="/img/davila.png" alt="" usemap="#davila" />
        <map name="davila">
          <area
            shape="rect"
            coords="0,0,200,50"
            alt="Computer"
            href="https://www.instagram.com/elegi4/?igshid=YmMyMTA2M2Y%3D"
          />
          <area
            shape="rect"
            coords="0,60,200,90"
            alt="Phone"
            href="https://www.instagram.com/p3pinot/?igshid=YmMyMTA2M2Y%3D"
          />
         <area
            shape="rect"
            coords="0,90,200,120"
            alt="Coffee"
            href="https://www.instagram.com/valeriabaret/?igshid=YmMyMTA2M2Y%3D"
          />  
        </map>
        </div>
        
        <a
          target="_blank"
          href="https://www.instagram.com/cristinamariarumin/?igshid=YmMyMTA2M2Y%3D"
          ><img src="/img/cristina.webp" alt=""
        /></a>
      </div>
      <div class="prensa_enlaces">
        <a target="_blank" href="https://www.instagram.com/isabelfcg/"
          ><img src="/img/isabel.webp" alt=""
        /></a>

        <a
          target="_blank"
          href="https://www.instagram.com/alvsmonster/?igshid=YmMyMTA2M2Y%3D"
          ><img src="/img/alvs.png" alt=""
        /></a>
        <a target="_blank" href="https://www.instagram.com/3819etc/"
          ><img src="/img/rgb.png" alt=""
        /></a>
      </div>
    </div>
    <div class="prensa_navigation">
      <MenuNavegacion linkUrl="instalaciones" />
    </div>
  </div>
</template>
<style lang="scss" scoped>
.prensa_main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  background-image: url("/img/fondo_puerta.webp");
  background-size: cover;
  padding: 1em;
  @include tablet-grande() {
    min-height: 100vh;
    //max-width: 900px;
    margin: 0 auto;
    //margin-top: 4em;
  }
}
.prensa_content {
  @include tablet-grande() {
    display: flex;
    align-items: center;
    flex-direction: row;
    gap: 2em;
    //margin-top: 3em;
    padding: 0 1em;
    max-width: 1200px;
    margin: 0 auto;
  }
}
.prensa_enlaces {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1em;
  @include tablet-grande() {
    grid-template-rows: 1fr 1fr 1fr;
    padding: 2em;
  }
}
.prensa_navigation {
  @include tablet-grande() {
    margin-top: 3em;
  }
}
</style>
