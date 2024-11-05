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

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  h3 {
    position: relative;
    left: 0;
    margin-bottom: 10px;
  }

  .nav {
    flex-direction: column;
    gap: 10px;
  }

  .nav-link {
    font-size: 16px;
    text-align: center;
  }
}

@media (max-width: 576px) {
  .navbar {
    padding: 5px 10px;
  }

  .nav-link {
    font-size: 14px;
  }

  h3 {
    font-size: 18px;
  }
}
</style>
