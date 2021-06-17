<template>
  <div class="container-fluid d-none d-lg-block" style="min-height:98vh" id="sec_0">
    <div class="row">
      <div class="a"></div>
      <div class="b"></div>
      <a role="button" class="font-weight-bold mx-auto btn btn-outline-light d-none d-md-block grid" @click="scrollMeTo('abm')"
        style="font-size:2rem; width:20vw; z-index:999; margin-top:42vh;">ABOUT ME</a>
    </div>
  </div>
  <div class="container mx-auto" style="margin-top:5vh;" ref="abm">
    <div class="row">
        <div class="card mb-3" style="max-width: 600px;">
            <div class="row no-gutters">
                <div class="col-md-4">
                <img src="../assets/img/profile.jpg" class="img-thumbnail mt-3" alt="">
                </div>
                <div class="col-md-8">
                <div class="card-body">
                    <p class="font-weight-bold" style="font-size:1.5rem; font-family:Nunito Sans;">吳品頤</p>
                    <p class="text-muted">WU PINYI</p>
                    <hr>
                    <p class="card-text">Skills and Abilities:HTML5、CSS、javascript、jQuery、vue.js、anjular.js、react.js、node.js、Bootstrap、python、PHP、C、C++、C#、Photoshop、After Effect、Illustrator</p>
                    <p class="font-weight-bold" style="font-size:1.5rem; font-family:Nunito Sans;">尋找後端or全端工程師職缺</p>
                    <div class="text-sm-center text-md-left">
                        <a class="btn-social mr-2" href="https://github.com/WuPinYi" style="text-decoration:none; color:black;"><i class="fab fa-github"></i></a>
                        <a class="btn-social mr-2" href="https://www.linkedin.com/in/wupinyi/" style="text-decoration:none; color:black;"><i class="fab fa-linkedin"></i></a>
                        <a class="btn-social mr-2" href="mailto:t104590020@ntut.org.tw" style="text-decoration:none; color:black;"><i class="far fa-envelope"></i></a>
                        
                    </div>
                </div>
                </div>
            </div>
        </div>
    </div>
    </div>

    <Education/>
</template>

<script>
import $ from 'jquery'
import Education from '@/components/Education.vue'
export default {
  components: {
    Education
  },
  methods: {
    scrollMeTo(refName) {
      var element = this.$refs[refName];
      var top = element.offsetTop;

      window.scrollTo(0, top);
    }
  },
  mounted() {
    $("body").mousemove(function (event) {
      var mouseX = event.pageX
      // var windowWidth = $(window).width() / 2
      // if(mouseX>=$(window).width()*0.2&&mouseX<=$(window).width()*0.8){
      $('.b').css("width", mouseX)
      // }
    });
    $(document).ready(function() {
    $(".dropdown-toggle").dropdown();
});
  }
}
</script>

<style scoped>
div.a, div.b{
  position: absolute;
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
  height: 100vh;
  width: 100%;
}
div.a:hover{
  cursor: col-resize;
}
div.b:hover{
  cursor: col-resize;
}
.a{
  background-image: url('../assets/img/me.jpg');
}
.b{
  background-image: url('../assets/img/meSketch.jpg');
}



*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-size: 62.5%;
}
body {
  padding: 2rem;
  background-color: #15202b;
  color: white;
  font-family: "Inter", sans-serif;
}

.heading {
  font-size: 4rem;
  text-align: center;
  margin-bottom: 3rem;
  text-shadow: 3px 4px 5px pink;
}

.container {
  perspective: 1000px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}

.item {
  transform: rotateX(45deg) scale(0.7);
  background-color: #192734;
  border-radius: 0.4rem;
  overflow: hidden;
  cursor: pointer;
  width: 30%;
  transition: 0.5s all ease;
  box-shadow: 0px 20px 50px #555;
}
.item:hover {
  cursor: pointer;
  transform: rotate(0deg) scale(1);
  transition: 0.5s all ease;
  z-index: 400;
  box-shadow: 0 2px 2px rgba(0, 0, 0, 0.16);
}
.card__img {
  display: block;
  width: 100%;
  height: 18rem;
  object-fit: cover;
}
.card__content {
  padding: 3rem 3rem;
}
.card__header {
  font-size: 3rem;
  font-weight: 500;
  color: #fff;
  margin-bottom: 1.5rem;
}
.card__text {
  font-size: 1.5rem;
  letter-spacing: 0.1rem;
  line-height: 1.7;
  color: #8899a6;
  margin-bottom: 2.5rem;
}
.card__btn {
  display: block;
  width: 100%;
  padding: 1.5rem;
  font-size: 2rem;
  text-align: center;
  color: #3363ff;
  background-color: #e6ecff;
  border: none;
  border-radius: 0.4rem;
  transition: 0.2s;
  cursor: pointer;
}
.card__btn span {
  margin-left: 1rem;
  transition: 0.2s;
}
.card__btn:hover,
.card__btn:active {
  background-color: #dce4ff;
}
.card__btn:hover span,
.card__btn:active span {
  margin-left: 1.5rem;
}

@media (max-width: 992px) {
  .item {
    width: 45%;
  }
}

@media (max-width: 768px) {
  .item {
    width: 80%;
  }
}

</style>