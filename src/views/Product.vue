<template>
  <div class="flex-container">
    <div class="col-md-6">
    <div class="image col">
        <div class="pro-img-details">
            <img src="http://thevectorlab.net/flatlab/img/product-list/pro-thumb-big.jpg" alt="">
        </div>    
    </div>
    </div>
    <div class="col-md-6">
     <div class="info">
              <h4 class="pro-d-title">
                  <a href="#" class="">
                      product name
                  </a>
              </h4>
              <p>
                  Praesent ac condimentum felis. Nulla at nisl orci, at dignissim dolor, The best product descriptions address your ideal buyer directly and personally. The best product descriptions address your ideal buyer directly and personally.
              </p>
              <div class="product_meta">
                  <span class="posted_in"> <strong>Categories:</strong> <a rel="tag" href="#">text</a>, <a rel="tag" href="#">text</a>, <a rel="tag" href="#">text</a>, <a rel="tag" href="#">text</a>.</span>
                  <span class="tagged_as"><strong>Tags:</strong> <a rel="tag" href="#">text</a>, <a rel="tag" href="#">text</a>.</span>
              </div>
              <div class="m-bot15">
                 <strong>Price : </strong> <span class="amount-old">$544</span> 
              </div>
              <div class="form-group m-bot15">
                  <strong>Quantity </strong>
                  <input type="quantiy" placeholder="1" class="quantity">
              </div>
              <p>
                  <button class="btn btn-round btn-danger" type="button"><i class="fa fa-shopping-cart"></i> Add to Cart</button>
              </p>
       </div>
      </div>    

  </div>
</template>
<style scoped>
.flex-container{
    display: flex;
    box-sizing: border-box;
    justify-content: space-between;
    flex-basis: 10px;
    margin: 25px;
    }
.quantity {
    width: 120px;
}
  .product_meta {
    border-top: 1px solid #eee;
    border-bottom: 1px solid #eee;
    padding: 10px 0;
    margin: 15px 0;
}

.product_meta span {
    display: block;
    margin-bottom: 10px;
}

</style>
<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

