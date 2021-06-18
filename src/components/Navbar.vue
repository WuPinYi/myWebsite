<template>
  <nav class="navbar fixed-top navbar-expand-lg navbar-light bg-transparent w-100 ng-scope" style="z-index:99999; min-height:6vh;">
  <div class="container">
    <a class="col-3 navbar-brand m-0 p-0 mr-3" href="index.html"><img class="img-fluid" src="../assets/img/signature.png"></a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link" href="index.html">HOME <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Projects
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
          <h6 class="dropdown-header">Website</h6>
          <a class="dropdown-item" @click="goTo()">BOSS</a>
          <a class="dropdown-item" href="#">BUSPLAY</a>
          <h6 class="dropdown-header">Game</h6>
          <a class="dropdown-item" href="#">Raise Your red flag</a>
        </div>
      </li>
      </ul>
    </div>
  </div>
</nav>
</template>

<script>
export default {
    name: 'Navbar',
    methods:{
      goTo(){
      this.$router.push('/Boss'); 
    }
  }
}
</script>

