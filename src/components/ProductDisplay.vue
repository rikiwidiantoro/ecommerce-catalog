<template>
  <div class="display-product">
    
    <div class="card">
      <div class="gambar">
        <img src="" alt="Gambar">
      </div>
      <div class="container">
        <h3><b>John Doe</b></h3>
        <p>Architect & Engineer</p>
        <hr>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consectetur quos provident quisquam voluptatem necessitatibus ex, aperiam nisi doloribus soluta molestias?</p>
        <hr>
        <p>$20.99</p>
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
  name: 'HelloWorld'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .display-product {
    margin: 100px auto;
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
  }

  .gambar {
    flex: 1;
    width: 25%;
    padding: 5px 20px;
  }

  /* On mouse-over, add a deeper shadow */
  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  }

  /* Add some padding inside the card container */
  .container {
    flex: 2;
    padding: 5px 20px;
    width: 75%;
    text-align: left;
    margin-bottom: 20px;
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
