<template>
  <div>
   <div class="header pt-6 relative ">
      <navbar />
       <hr class="line-heder w-full mt-6 relative z-10">
      <header-content/>
   </div>
     <about />
     <question />
     <statistica />
     <fresh />
     <the-footer />
  </div>
</template>

<script>
import HeaderContent from '../components/headerContent.vue'
import Navbar from '../components/Navbar.vue'
export default {
  components: { Navbar, HeaderContent },
  name: 'IndexPage'
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  font-family: 'Cera PRO';
}

.header{
  position: relative;
  background-image: url(../static/header/main-img.png);
  background-size: cover;
  padding-bottom: 280px;
}
.header::before{
  content: "";
  position: absolute;
  width: 100%;
  top: 0;
  height: 730px;
  background: linear-gradient(296deg, rgba(3, 20, 16, 0) -12.71%, rgba(3, 20, 16, 0.34) -12.7%, rgba(3, 20, 16, 0.72914) 38.36%, rgba(3, 20, 16, 0.879618) 60.67%, #031410 100%);
  

}
.line-heder{
  background: #354340;
  transform: matrix(1, 0, 0, -1, 0, 0);
}
.container{
  max-width: 1212px;
  margin: 0 auto;
}
</style>
