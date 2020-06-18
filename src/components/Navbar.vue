<template>
  <div >
      <nav class="navbar navbar-expand-lg " style="background-color: #69217E; padding-left:50px;">
  <a class="navbar-brand" href="/">
      <img class="mr-3" :src="require('../assets/abhimanyu logo.png')" height="40"/>  
  </a>
     <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <form class="center-block">
      <input class="form-control" type="search" placeholder="Search Here
      " required
    size="70" aria-label="Search">
    </form>
      <a class="navbar-brand" href="#">
      <img class="mr-3" :src="require('../assets/save.png')" height="30"/>  
  </a>
    <a class="navbar-brand" href="/Cart">
      <img class="mr-3" :src="require('../assets/cart.png')" height="30"/>  
  </a>
  </div>
</nav>
<div class="menu">
<a class="nav-link nav-link-ltr"  href="/">Home</a>
<a class="nav-link nav-link-ltr" href="#">fruit</a>
<a class="nav-link nav-link-ltr" href="#">veggies</a>
<a class="nav-link nav-link-ltr" href="#">diary</a>
<a class="nav-link nav-link-ltr" href="/about">others</a>
</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.center-block {
  display: block!important;
  margin-right: auto!important;
  margin-left: auto!important;
}
.menu {
  border-bottom: 1px solid #BBBBBB;
  left: 150px;
    padding: 0;
  margin: 0;
 
}

.nav-link {
  font-weight: bold;
  font-size: 14px;
  text-transform: uppercase;
  text-decoration: none;
  color: #031D44;
  padding: 20px 0px;
  margin: 0px 20px;
  display: inline-block;
  position: relative;
  opacity: 0.75;
}

.nav-link:hover {
  opacity: 1;
}

.nav-link::before {
  transition: 300ms;
  height: 5px;
  content: "";
  position: absolute;
  background-color: #031D44;
}

.nav-link-ltr::before {
  width: 0%;
  bottom: 10px;
}

.nav-link-ltr:hover::before {
  width: 100%;
}

</style>
