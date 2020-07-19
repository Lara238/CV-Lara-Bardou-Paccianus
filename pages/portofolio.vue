<template>
  <div class="container">
   <div class="header">
      <h1> Hello Portofolio </h1>
      <NuxtLink to="/">
        Click here to go to the HomePage
      </NuxtLink>
    </div>
    <div class="grid-container"> 
      <img class="grid-item" src="../assets/horse.jpeg"/>
      <img class="grid-item" src="../assets/game.jpeg"/>
      <img class="grid-item" src="../assets/japan.jpeg"/>
      <img class="grid-item" src="../assets/photo.jpeg"/>
      <img class="grid-item" src="../assets/rock.jpeg"/>
      <img class="grid-item" src="../assets/space.jpeg"/>
    </div>

  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  padding: 10px;
  grid-template-areas:
    'header header header header header header'
    'menu main main'
    'menu footer footer footer footer footer';
}
.grid-item {
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  text-align: center;
  width: 100%;
  height: auto;
  border-radius: 8px;
}

.header {
  grid-area: header;
}
</style>
