<template id="app">

    <header class="header">
      <a href="#" class="logo"><img src="/src/assets/logo.png" alt=""></a>
      <nav class="nav">
        <a href="#" class="nav__link">{{l1}}</a>
        <a href="#" class="nav__link">{{l2}}</a>
        <a href="#" class="nav__link">{{l3}}</a>
        <a href="#" class="nav__link">{{l4}}</a>
      </nav>
    </header>

</template>

<script>
export default {
  data: function() {
    return {
      l1:'About',
      l2:'Downloads',
      l3:'Plans',
      l4:'Contact'
      
}
}}
</script>

<style scoped>

  .header{
  padding-top: 25px;
  display:flex;
  justify-content: space-between;
  align-items: center;
}
.nav__link{
  margin-left: 20px;
  font-size: 18px;
  font-weight: 700;
  line-height: 42px;

}
a{
  color: #ffffff;
  text-decoration: none;
}

</style>