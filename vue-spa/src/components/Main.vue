<template>
  <main class="main">
    <div class="main-text">
      <p class="uppertext">{{ uppertext }}</p>
      <p class="subtext">{{ subtext }}</p>
    </div>
    <div class="main-chekbox">
      <div class="aboutus">{{ bigtext }}</div>
      
      <ul class="cheklist">
        <li class="list">{{ li1 }}</li>
        <li class="list">{{ li2 }}</li>
        <li class="list">{{ li3 }}</li>
        
      </ul>
      
      <div class="container__btn">
        <!-- <button class="btn">{{ btn }}</button> -->
        <div class="btn">{{btn}}</div>
      </div>
      <img src="/src/assets/Macbook.png" alt="" class="img">
    </div>
  </main>
</template>

<script>
export default {
  data: function() {
    return {
      uppertext: "free resources",
      subtext: "just download it",
      bigtext:
        "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
      li1: "Duis aute irure dolor in reprehenderit in voluptate.",
      li2: "Excepteur sint occaecat cupidatat non proident.",
      li3: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem.",
      btn: "Read more"
    };
  }
};
</script>

<style scoped>
.btn:active{
		transform:translateY(4px) ;
}
.main {
  margin-top: 628px;
}
.main-text {
  display: flex;
  justify-content: center;
  position: relative;
}
.uppertext {
  margin: 0;
  font-size: 114px;
  font-weight: 400;
  line-height: 150.61px;
  text-transform: uppercase;
}
.img {
  position: absolute;
  left: 0;
  bottom: 0;
  margin-left: 430px;
}
.subtext {
  text-transform: uppercase;
  margin: 0;
  color: #25365d;
  font-size: 25px;
  line-height: 32px;
  font-weight: 800;
  position: absolute;
  left: 0;
  bottom: 0;
  margin-bottom: 48px;
  margin-left: 23px;
}
.main-chekbox {
  position: relative;
  display: block;
  margin-left: 40px;
  max-width: 696px;
}
.aboutus {
  color: #5a5a5a5a;
  font-size: 17px;
  line-height: 32px;
  margin-bottom: 30px;
}
.cheklist {
  color: #93aac9;
  list-style-type: none;
  margin: 0;
  padding: 0;
  font-size: 16px;
  line-height: 20px;
}
.list:after {
  content: "";
  display: block;
  background-image: url("/src/assets/right.svg");
  width: 17px;
  height: 17px;
  float: left;
  margin-right: 18px;
}
.container__btn {
  display: flex;
  margin-top: 60px;
  justify-content: flex-start;
}

.btn {
  position: relative;
  border-radius: 28px;
  background-color: #25365d;
  color: #ffffff;
  font-size: 18px;
  font-weight: 700;
  line-height: 17px;
  outline: none;
  border: none;
  padding: 19px 58px 22px 64px;
  cursor: pointer;
}
.container__btn:after {
  content: "";
  display: block;
  background-image: url("/src/assets/Macbook.png");
}
@media (max-width:1659px) {
  .img{
    display: none;
  }
}
@media (max-width:1090px) {
  .uppertext{
    font-size: 90px;
    
  }
  .subtext{
    margin-left: 30px;
  }
  .main-text {
    justify-content: flex-start;
  }
}
@media (max-width:864px) {
  .uppertext{
    font-size: 80px;
    
  }
  .subtext{
    margin-left: 30px;
  }
 
}
@media (max-width:770px) {
  .uppertext{
    font-size: 70px;
    
  }
  .subtext{
    margin-left: 30px;
  }
   .container__btn{
    justify-content: center;
  }
 
}
@media (max-width:676px) {
  .uppertext{
    font-size: 60px;
    
  }
  .subtext{
    margin-left: 30px;
  }
 
 
}
</style>
