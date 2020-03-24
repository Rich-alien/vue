<template>
<div  class="container">
      <div class="header-text">
       {{uppertext}}
        </div>
        <div class="undertext">
          <span>{{undertext}}</span>
        </div>
</div>
</template>

<script>
export default {
  data: function() {
    return {
        uppertext:'Download this template for free',
        undertext:`Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
         eiusmod tempor incididuntut labore et dolore magna aliqua.Ut enim ad minim veniam, 
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.`
    }
  }
}
</script>

<style scoped>

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
  font-size: 45px;
  line-height: 32px;
  font-weight: 400;
}
.undertext{
  margin-top: 62px;
  color: #5a5a5a;
  text-align: center;
  margin-bottom: 71px;
}
@media (max-width:946px) {
  .header-text{
    font-size: 34px;
  }
}
@media (max-width:719px) {
  .header-text{
    font-size: 27px;
  }
}
</style> 