<template>
<div>
<div class="container">
  <div class="container">
  <div class="row">
    <div class="col">
        <div class="main">
            <div class="card">
                <div class="image btn btn-outline-secondary">
                      <img src="https://imageresizer.static9.net.au/_AC5YNG0fryCEQuu3A-ojFBQrF4=/600x338/smart/https%3A%2F%2Fprod.static9.net.au%2F_%2Fmedia%2FNetwork%2FImages%2F2017%2F05%2F05%2F08%2F40%2F170505coach_vegetables.jpg" width="170" height="158">
                </div>
            </div>
            <div class="card">
                            <div class="image btn btn-outline-secondary">
                                  <img src="https://5.imimg.com/data5/TE/UT/MY-925184/dry-fruits-and-nuts-testing-500x500.png" width="170" height="158">
                            </div>
                    </div>
            <div class="card">
                <div class="image btn btn-outline-secondary">
                      <img src="https://media.istockphoto.com/photos/red-apple-with-leaf-picture-id683494078?k=6&m=683494078&s=612x612&w=0&h=aVyDhOiTwUZI0NeF_ysdLZkSvDD4JxaJMdWSx2p3pp4=" width="170" height="158">
                </div>
            </div>
            <div class="card">
                <div class="image btn btn-outline-secondary">
                      <img src="https://image.shutterstock.com/image-vector/cow-260nw-238683511.jpg" width="170" height="158">
                </div>
            </div>
        </div>
    </div>
  </div>
</div>
<div id="app">
<div class="rfu">
        <h1> Fruits</h1>
       
      <div class="flex-container">
        
        <div v-bind:key="category.id" v-for="category in category" >
           <div class="flex-item" >
              <img  im in category.images :key="im" :src="im" width="200" height="150" class="img" />
               <a href="/Product">
              <legend>{{category.title}}</legend> 
              <h5>Price: {{category.price}}</h5>
               </a>
              <div class="buttons">
              <button class="btn btn-primary btn-sm button-a" >add to cart</button>
              <button class="btn btn-success btn-sm button-b" >save for later</button>
              </div>
           </div>
        </div>
      
     </div>
      

       <div id="demo" class="carousel slide sec3" data-ride="carousel">

  <!-- Indicators -->
  <ul class="carousel-indicators">
    <li data-target="#demo" data-slide-to="0" class="active"></li>
    <li data-target="#demo" data-slide-to="1"></li>
    <li data-target="#demo" data-slide-to="2"></li>
  </ul>

  <!-- The slideshow -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="https://www.w3schools.com/bootstrap4/la.jpg" height="100%" width="100%" alt="Los Angeles">
 <div class="carousel-caption">
    <h3>Los Angeles</h3>
    <p>We had such a great time in LA!</p>
  </div>
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="https://www.w3schools.com/bootstrap4/la.jpg" alt="Chicago">
 <div class="carousel-caption">
    <h3>Los Angeles</h3>
    <p>We had such a great time in LA!</p>
  </div>
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="https://www.w3schools.com/bootstrap4/la.jpg" alt="New York">
 <div class="carousel-caption">
    <h3>Los Angeles</h3>
    <p>We had such a great time in LA!</p>
  </div>
    </div>
  </div>

  <!-- Left and right controls -->
  <a class="carousel-control-prev" href="#demo" data-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </a>
  <a class="carousel-control-next" href="#demo" data-slide="next">
    <span class="carousel-control-next-icon"></span>
  </a>

</div>

     <div class="rfu" >
        <h1> Vegetables</h1>
      <div class="flex-container">
        <div v-bind:key="category.id" v-for="category in category" >
           <div class="flex-item" >
              <img  im in category.images :key="im" :src="im" width="200" height="150" class="img" />
              <legend>{{category.title}}</legend> 
              <h5>Price: {{category.price}}</h5>
              
              <div class="buttons">
              <button class="btn btn-primary btn-sm button-a" >add to cart</button>
              <button class="btn btn-success btn-sm button-b" >save for later</button>
              </div>
           </div>
        </div>
     </div>
     </div>
</div>
</div>
</div>
</div>
</template>
<style scoped>


*{
 margin: 0px;
 padding: 0px;
}

.main{

 margin: 2%;
}

.centered {
  position: absolute!important;
  top: 80%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.card{
    display: inline-flex;
     width: 20%;
     box-shadow: 2px 2px 20px black;
     border-radius: 5px; 
     margin: 2%;
    }

.image img{
  width: 100%;
  border-top-right-radius: 5px;
  border-top-left-radius: 5px;
  
 }
.carousel-caption{
  padding-bottom: 250px;
 left: -50%;
}
.rfu{
 margin: 0px;
 padding: 0px;
 margin-bottom: 20px;
}

h1{
  display: flex;
  padding: 15px;
}
.img{
  padding: 10px;
}
.buttons{
display:flex;
justify-content: center;
flex-direction: column;
padding: 5px;
justify-content: space-between;
}
.button-a{
flex: 1;
margin-bottom: 10px;

}
.button-b{
  flex: 1;

}
.flex-item{
    height: 350px;
    width: 250px;
    background-color: white;
    text-align: center;
    margin:  auto;
    border: 1px solid #ccc;
    box-shadow: 0px 5px 25px #aaa;
    border-radius: 10px;
}


.flex-container{
    display: flex;
    box-sizing: border-box;
    justify-content: space-between;
    flex-basis: 10px;
    }

  .sec3{
    margin-top: 20px;
}
</style>
</style>

<script>
import axios from "axios";

export default {
  name: 'app',
  data() {
    return{
      category: []
    };
  },
  async created(){
    try {
      const res = await axios.get(`http://localhost:3000/category`);
      this.category = res.data;
    }catch(e){
      console.error(e);
    }
  }
};
</script>
