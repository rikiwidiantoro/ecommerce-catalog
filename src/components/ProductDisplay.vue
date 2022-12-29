<!-- eslint-disable vue/no-multiple-template-root -->
<template>
  <div class="display-product">
    
    <div class="card" v-for="product in products" :key="product.id">
      <div class="gambar">
        <img :src="product.image" alt="gambar" width="200px">
      </div>
      <div class="container">
        <h2><b>{{ product.title }}</b></h2>
        <div class="rating">
          <span>{{ product.category }}</span>
          <span class="rat">{{ product.rating.rate }}/5</span>
        </div>
        <hr>
        <p style="text-align: justify;">{{ product.description }}</p>
        <hr>
        <h3>${{ product.price }}</h3>
        <div class="tombol">
          <button style="margin-right: 10px; background-color: #720060; color: white;">
            <a href="" style="color: white; text-decoration: none;">Buy now</a>
          </button>
          <button style="border-color: #720060; background-color: white;">
            <a href="" style="color: #720060; text-decoration: none;">Next product</a>
          </button>
        </div>
      </div>
    </div>
  </div>
  
</template>

<script>
export default {
  data() {
    return{
      products: []
    }
  },
  mounted() {
    fetch('https://fakestoreapi.com/products')
    .then(res => res.json())
    .then(data => this.products = data)
    // eslint-disable-next-line no-undef
    .catch(err = console.log(err.message))
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .display-product {
    margin: 0px auto 100px;
    width: 1200px;
    height: 500px;
  }
  .card {
    /* Add shadows to create the "card" effect */
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    display: flex;
    background-color: #FFFFFF;
    border-radius: 5px;
    margin-bottom: 30px;
  }

  .gambar {
    flex: 1;
    width: 25%;
    padding: 25px 0px;
  }

  /* On mouse-over, add a deeper shadow */
  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  }

  /* Add some padding inside the card container */
  .container {
    flex: 2;
    padding: 5px 50px 5px 0px;
    width: 75%;
    text-align: left;
    margin-bottom: 20px;
  }

  .rating .rat {
    float: right;
  }

  button {
    width: 46%;
    height: 30px;
    border-radius: 3px;
    border-color: #720060;
  }
  button:hover {
    cursor: pointer;
  }

  hr {
    background-color: #DCDCDC;
  }
</style>
