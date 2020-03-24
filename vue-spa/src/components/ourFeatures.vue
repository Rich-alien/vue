<template>
    <div class="container">
         <p class="header-text">
       {{tHeader}}
        </p>
        <div class="main">
                  <div class="left__features">
                    <div class="block-left">
            <h2 class="text1">{{f1}}</h2>
          <span class="span">
            {{tSpan}}
          </span>
          </div>
                    <div class="block-left">
            <h2 class="text2">{{f2}}</h2>
          <span class="span">
            {{tSpan}}
          </span>
          </div>
        </div>

        <div class="notebook">
            <div class="left-notebook">
              <img src="/src/assets/Macbook_1.png" alt="" class="Limg">
            </div>
             <div class="right-notebook">
              <img src="/src/assets/Macbook_2.png" alt="" class="Rimg">
            </div>
        </div>

        <div class="right__features">
          <div class="block-right">
            <h2 class="text3">{{f3}}</h2>
          <span class="span">
            {{tSpan}}
          </span>
          </div>

          <div class="block-right">
            <h2 class="text4">{{f4}}</h2>
          <span class="span">
            {{tSpan}}
          </span>
          </div>
        </div>
        </div>

    </div>


</template>

<script>
export default {
  data: function() {
    return {
        tHeader:'check our features',
        tSpan:'Duis aute irure dolor in reprehenderit in voluptate. Excepteur sint occaecat.',
        f1:'Feature 1',
        f2:'Feature 2',
        f3:'Feature 3',
        f4:'Feature 4',
    }
  }
}
</script>

<style scoped>
/* .left-notebook{
  border-right: 1px solid #cecece;
} */
.notebook{
  position: relative;
}
.left-notebook:after{
  position: absolute;
  content: "";
	display: block;
  background-image: url("/src/assets/Change.png") ;
  background-repeat: no-repeat;
  width: 64px;
  height: 593px;
  left: 46%;
  top: -13%;

}
.container{ 
  margin-top: 155px ;
  margin-bottom: 174px;
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
}
.header-text{
  margin-bottom: 147px;
  margin-top: 0;
  text-transform: uppercase;

  color: #25365d;
  font-size: 25px;
  line-height: 32px;
  font-weight: 800;
}
h2{
  color: #25365d; 
  font-size: 22px;
  line-height: 31px;
  border-bottom: 1px solid #ff2868;
}
/* .text:after:first-child{
  content: "";
	display: block;
	background-image: url("/src/assets/lenght1.svg");
  width: 318px;
	height: 96px;
  right: 0;
  bottom: 0;
} */
.text2:after{
  position: absolute;
  content: "";
	display: block;
	background-image: url("/src/assets/Grupa_9.png") ;
  background-repeat: no-repeat;
  width: 318px;
	height: 96px;
  left: 117px;
  bottom: 44px;
  z-index: 3;

}
.text1:after{
   z-index: 3;
  position: absolute;
  content: "";
	display: block;
	background-image: url("/src/assets/Grupa_1.png") ;
  background-repeat: no-repeat;
  width: 318px;
	height: 96px;
  left: 117px;
  bottom: -22px;
}
.text3:after{
  position: absolute;
  content: "";
	display: block;
	background-image: url("/src/assets/Grupa_2.png") ;
  background-repeat: no-repeat;
  width: 318px;
	height: 96px;
  right: 117px;
  bottom: -22px;
}
.text4:after{
  position: absolute;
  content: "";
	display: block;
	background-image: url("/src/assets/Grupa_3.png") ;
  background-repeat: no-repeat;
  width: 318px;
	height: 96px;
  right: 110px;
  bottom: 16px;
}

.block-left{
  position: relative;
}
.block-right{
  position: relative;
}
.span{
  color: #5a5a5a;
  font-size: 14px;
}
.main{
  display: flex;
  flex-direction: row;
}
h2{
  width: 100%;
  margin: 0;
}
.left__features{
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  max-width: 191px;
}
.right__features{
    display: flex;
  flex-direction: column;
  justify-content: space-around;
  text-align: end;
  max-width: 191px;
}
.notebook{
  display: flex;
}
@media (max-width: 1188px) {
.text1:after{
  bottom: -5px;
}
.text2:after{
  bottom: 62px;
}
.text3:after{
  bottom: -5px;
}
.text4:after{
  bottom: 34px;
}

}
@media (max-width: 1187px) {
.text1:after{
  bottom: 13px;
}
.text2:after{
  bottom: 80px;
}
.text3:after{
  bottom: 13px;
}
.text4:after{
  bottom: 52px;
}

}
@media (max-width: 1187px) {
.right__features{
display: none;
}
.left__features{
display: none;
}
}

</style> 