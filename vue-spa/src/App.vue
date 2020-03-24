<template>
  <div id="app">
    
    <div class="container">
      <img class="bird" src="/src/assets/bird.png" alt="">
        <headerPage/>
        <headerMain/>
        <btnDownload/>
        <Main/>
    </div>
        <achivment/>
    <div class="container">
        <ourFeatures/>
    </div>
    <plans/>
     <div class="container">
        <footerSite/>
        <div class="btn-footer">
          <btnDownload/>
        </div>
    </div>
  </div>
</template>

<script>
import headerPage from "./components/headerPage";
import headerMain from "./components/headerMain";
import btnDownload from "./components/btnDownload";
import Main from "./components/Main";
import achivment from "./components/achivment";
import ourFeatures from "./components/ourFeatures";
import plans from "./components/plans";
import footerSite from "./components/footerSite";
// import { MLInstaller, MLCreate, MLanguage } from 'vue-multilanguage';
export default {
  name: "App",
  components: {
    headerPage,
    headerMain,
    btnDownload,
    Main,
    achivment,
    ourFeatures,
    plans,
    footerSite,
  }
};
</script>

<style>
#app {
  
  background: #070506 url("../src/assets/bgp.png") no-repeat right  top;
  background-size: cover;
  color: white;
  font-family: 'Roboto', sans-serif ;
}
</style>
<style scoped>
   .container{
     position: relative;
  font-family: "1";
  width: 90%;
  max-width: 1060px; 
  margin: auto;
	}
  .btn-footer{
    padding-bottom: 510px;
  }
  .bird{
    display: none;
    position: absolute;
    height: 50px;
    width: 50px;
    animation: move 10s linear infinite;
  }
  @keyframes move {
    10%{
      transform: translateX(1080px) translateY(10px);
    }
    89%{
      transform: rotateY(180deg);
    }
    90%{
      transform: translateX(0px) translateY(10px);
      
    }
   
  }

</style>
