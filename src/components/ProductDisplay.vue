<template>
  <div class="display-product">
    
    <div class="card">
      <div class="gambar">
        <img src="" alt="Gambar">
      </div>
      <div class="container">
        <h4><b>John Doe</b></h4>
        <p>Architect & Engineer</p>
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
    width: 1000px;
    height: 500px;
  }
  .card {
    /* Add shadows to create the "card" effect */
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    display: flex;
  }

  .gambar {
    flex: 1;
    width: 20%;
    padding: 2px 16px;
  }

  /* On mouse-over, add a deeper shadow */
  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  }

  /* Add some padding inside the card container */
  .container {
    flex: 2;
    padding: 2px 16px;
    width: 80%;
  }
</style>
