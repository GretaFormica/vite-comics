<script setup>

</script>

<template>
  
  <header>

    <div class="container">

      <div class="flex">

        
        <img src="../../vue-dc-comics-1/img/dc-logo.png">
        
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
        </ul>
        
      </div>

    </div>

  </header>

</template>

<style lang="scss">

header{
  height: 80px;
}

.container{
  max-width: 1200px;
  margin: 0 auto;
  height: 100%;
}

.flex{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;

  img{
    width: 50px;
  }
}

ul {
  list-style-type: none;

  li{
    display: inline-block;
    margin: 0 0.5rem;

    a{
      color: inherit;
      text-decoration: none;
    }
  }
}

</style>
