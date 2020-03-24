<template>
<main class="plans">
<div class="container">
         <p class="header-text">
       {{tHeader}}
        </p>
        <p class="subtext">
          {{subtext}}
        </p>
<div class="price-block">
        <div class="block">
          <span class="block-subtext">{{p1}}</span>
          <div class="price-let">
          <span class="price">$25</span> <span class="currency">{{currency}}</span>
          </div>
          <span class="undertext">{{subtextBlock}}</span>
        </div>
        <div class="block">
          <span class="block-subtext">{{p2}}</span>
          <div class="price-let">
          <span class="price">$50</span><span class="currency">{{currency}}</span>
          </div>
          <span class="undertext">{{subtextBlock}}</span>


        </div>
        <div class="block">
          <span class="block-subtext">{{p3}}</span>
          <div class="price-let">
          <span class="price">$75</span><span class="currency">{{currency}}</span>
          </div>
          <span class="undertext">{{subtextBlock}}</span>
        </div>
</div>
          <div class="blue-women">
          <img src="/src/assets/call37.png" alt="">
          </div>
          <span class="go-quest">{{question}}</span>
          <div class="underQuest">{{questionUnder}}</div>
          <div class="contact">
          <a class="mail" href="mailto:suppor@free.com">suppor@free.com</a>
          <a class="tel" href="tel: +79372099245">+79 372 099 245</a>
          </div>

</div>
</main>
</template>

<script>
export default {
  data: function() {
    return {
        tHeader:'plans',
        subtext:`Lorem ipsum dolor sit amet, consectetur adipisicing elit,
         sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
         Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.`,
        currency: '/mon',
        subtextBlock:'Lorem ipsum dolor sit',
        question:'go questions?',
        questionUnder:`Contact our customer support team if 
        You have any further questions.
        We are here to help You out!`,
        p1:'Basic plan',
        p2:'professional plan',
        p3:'professional+ plan',
    }
  }
}
</script>

<style scoped>
.contact{
  margin-top: 71px;
  padding-bottom: 119px;
}
.mail:after{
  	content: "";
		display: block;
		background-image: url("/src/assets/mail59.png") ;
    background-repeat: no-repeat;
		width: 32px;
		height: 24px;
    float: left;
    padding-left: 11px;
		
}
.tel:after{
  	content: "";
		display: block;
		background-image: url("/src/assets/telephone46.png") ;
    background-repeat: no-repeat;
		width: 27px;
		height: 27px;
    float: left;
    padding-left: 11px;
		
}

a{
  color:#25365d;
  font-size: 22px;
  line-height: 30px;
  font-weight: 700;
  text-decoration: none;
}
.contact{
  display: flex;
  justify-content: space-between;
  min-width: 523px;
}
.go-quest{
  margin-top: 31px;
  text-transform: uppercase;
  color: #25365d;
  font-size: 22px;
  line-height: 36px;
  letter-spacing: 0.44px;
}
.underQuest{
   margin-top: 31px;
   color: #5a5a5a;
   text-align: center;
   max-width: 510px;
}
.blue-women{
  margin-top: 77px;
}
.price-block{
  width: 100%;
  display: flex;
  justify-content: space-between;
}
.block-subtext{
  padding-top: 25px;
  text-transform: uppercase;
  font-size: 18px;
  line-height: 36px;
  color: #5a5a5a;


}
.price{ 
  width: auto;
  color: #25365d;
  font-size: 72px;
  line-height: 36px;
}
.price-let{
  padding-top:59px;
}
.currency{
  color: #5a5a5a;
  font-size: 22px;
  line-height: 36px;
}
.undertext{
  color: #5a5a5a;
    font-size: 18px;
  line-height: 36px;
  padding-top: 50px;
  padding-bottom: 25px;
}
.block{
  display: flex;
  flex-direction: column;
  background-color:#ffffff;
  text-align: center;
  min-width: 330px;
}

.plans{
		background-color: #f7f9fd;
}
.container{ 
  max-width: 1030px; 
  margin: auto;
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
}
.header-text{

  margin-top: 152px;
  text-transform: uppercase;
  color: #25365d;
  font-size: 25px;
  line-height: 32px;
  font-weight: 800;
}
.subtext{
  
  font-size: 16px;
  line-height: 32px;
  color: #5a5a5a;
  text-align: center;
}
@media (max-width:1055px) {
  .price-block{
    flex-direction: column;
    align-items: center;
  }
  .block{
  display: flex;
  max-width: 330px;
  margin-top: 30px;
}
}
</style> 