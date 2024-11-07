<template>
  <header>
    <nav class="navbar navbar-expand-lg text-bg-secondary">
      <h3 class="nav"><i class="mdi mdi-chevron-left"></i>Solon/<i class="mdi mdi-chevron-right"></i></h3>
      <ul class="nav nav-underline">
        <li class="nav-item">
          <a class="nav-link active" href="#home">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#about">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#projects">Projects</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#contact">Contact</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>



<style scoped>

.navbar{
  display: flex;
  justify-content: center;
}

h3{
  font-family: 'Courier New', Courier, monospace;
  position: absolute;
  left: 5%;
  display: flex;
}

.nav-link{
  font-family: 'Playfair Display', sans-serif;
  font-weight: 600;
  color: #fff;
}

.nav-link:hover{
  color: #000;
}

@media (max-width: 599px){
  .navbar>h3{
    font-size: 2.5vh;
    left: 0;
  }

  .navbar>ul{
    font-size: 1.5vh;
    margin-left: 30vw;
  }

  .nav .nav-underline{
    margin-left: 2vw;
  }
}

/* @media (max-width: 599px){

} */
</style>
