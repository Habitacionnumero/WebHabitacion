<script setup>
import MenuNavegacion from '../components/MenuNavegacion.vue';
</script>
<script>
export default{
    data(){
        return{
            show: false,
        }
    }
}
</script>
<template>
    <div class="max-width padding-web">
    <div class="year_img">
        <video  @ended="show = !show" muted playsinline autoplay src="/img/papel.mp4"></video>
    </div>
    <div class="year_position" :class="{active: show}">
        
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/Cg6fCzTjaxy/?utm_source=ig_web_copy_link" target = "_blank">
                @tfpello
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CfrFeOvjPje/?utm_source=ig_web_copy_link" target = "_blank">
                @javier.montoro
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CegIRYEDygr/?utm_source=ig_web_copy_link" target = "_blank">
                @theetatthunkijjanukij
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CdQSDZaDHHm/?utm_source=ig_web_copy_link" target = "_blank">
                @adrianaberges
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CbxCsojjGbD/?utm_source=ig_web_copy_link" target = "_blank">
                @aida_salan
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/Ca17RrBqlFx/?utm_source=ig_web_copy_link" target = "_blank">
                @mora__carmen
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CZMyQ6iu9PH/?utm_source=ig_web_copy_link" target = "_blank">
                @guillermo.solas
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CX0weGGqS6H/?utm_source=ig_web_copy_link" target = "_blank">
                @lanutrialopez
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CWs8hbqqkVU/?utm_source=ig_web_copy_link" target = "_blank">
                @reflexin_ 
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CVhunaLjymi/?utm_source=ig_web_copy_link" target = "_blank">
                @esthermerinero
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CUe25b9Dkvj/?utm_source=ig_web_copy_link" target = "_blank">
                @barquero____
            </a>
        </div>
        <div class="year_position_a">
            <a href="https://www.instagram.com/p/CT6xzDCj-OF/?utm_source=ig_web_copy_link" target = "_blank">
                @kai.landre
            </a>
        </div>
    </div>
        <MenuNavegacion linkUrl="instalaciones"/>
    </div>
</template>
<style lang="scss" scoped>
.year_img{
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    //justify-content: center;
    position: relative;
    opacity: .8;
}
.year_position{
    display: flex;
    flex-direction: column;
    //justify-content: center;
    align-items: center;
    gap: 1em;
    position: absolute;
    top: 13em;
    left: 0;
    width: 100%;
    height: 100vh;
    font-weight: 900;
    font-size: .5em;
    color: #405e9d ;
    opacity: 0;
    transition: opacity .1s ease-in;
    @include mobile-xl(){
        font-size: .8em;
    }
    @include tablet(){
        font-size: .9em;
    }
}
.active{
    opacity: 1;
}
</style>