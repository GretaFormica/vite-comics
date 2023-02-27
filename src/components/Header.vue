<script setup>

</script>

<template>
  
  <header>

    <div class="container-h">

      <div class="flex">

        
        <img src="../../vue-dc-comics-1/img/dc-logo.png">
        
        <ul class="ul-h">
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

.container-h{
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

.ul-h{
    display: flex;

    li{
      &:hover{
        color:  rgb(68, 86, 226);
      }
    }
}



</style>
