<template>
  <main-navbar></main-navbar>
  <section>
    <div class="bg">
      <!-- <div class="container"> -->
      <div class="title text-center text-light">
        <img src="../assets/minecraft.png" class="img-fluid" alt="" />
      </div>
      <!-- </div> -->
      <!-- <div class="container"> -->
      <div class="server text-center">
        <img src="../assets/minecraftserver.png" class="img-fluid" alt="" />
      </div>
      <!-- </div> -->
    </div>
  </section>
  <latest-news></latest-news>
  <!-- introduction -->
  <div class="intro">
    <div class="container-fluid p-5 introduction">
      <div class="row apppp">
        
        <!-- <div class="col col-md-5 col-lg-4 mb-5">
          <div class="mb-5">
            <img src="@/assets/homepage/zombie.png" alt="create-picture" />
          </div>
          <div class="introbg1 text-light">
            <div>有時生存有時創造</div>
          </div>
        </div>
        <div class="col col-md-5 col-lg-4 mb-5">
          <div class="mb-5">
            <img src="@/assets/homepage/group.png" alt="play-picture" />
          </div>
          <div class="introbg2 text-light">
            <div>耐人尋味的關卡</div>
          </div>
        </div>
        <div class="col col-md-5 col-lg-4 mb-5">
          <div class="mb-5">
            <img src="@/assets/homepage/castle.png" alt="build-picture" />
          </div>
          <div class="introbg3 text-light">
            <div>蓋屬於自己的小天地！</div>
          </div>
        </div> -->
       
    <div class="product-wrap">
        <div class="product product1">1</div> 
    </div>         
    <div class="product-wrap">
        <div class="product0 product2">2</div> 
    </div>            
    <div class="product-wrap">
        <div class="product product3"><p>耐人尋味的關卡</p></div> 
    </div>      
  <div class="product-wrap">
        <div class="product0 product4">有時生存有時創造</div> 
    </div>         
    <div class="product-wrap">
        <div class="product product5">快開始你的麥塊吧!</div> 
    </div>            
    <div class="product-wrap">
        <div class="product0 product6">6</div> 
    </div>    
  <div class="product-wrap">
        <div class="product product7">7</div> 
    </div>         
    <div class="product-wrap">
        <div class="product0 product8">8</div> 
    </div>            
    <div class="product-wrap">
        <div class="product product9">蓋屬於自己的小天地！</div> 
    </div>    

      </div>
    </div>
  </div>
  <!-- icons -->
  <div id="info" class="container p-5">
    <div class="row fw-bold">
      <div class="col-md-6 col-sm-12 row text-center mb-5">
        <div class="title mb-5 text-center fs-1 fw-bold">社群平台</div>
        <a class="col-6" href="https://www.facebook.com/codedriven/"
          ><img src="@/assets/homepage/fbicon.png" alt="粉專"
        /></a>
        <a class="col-6" href=""
          ><img src="@/assets/homepage/discord.png" alt="discord"
        /></a>
      </div>
      <div class="col-md-6 col-sm-12 row text-center mb-5">
        <div class="title mb-5 text-center fs-1 fw-bold">合作夥伴</div>
        <a class="col-6" href="https://www.sce.pccu.edu.tw/"
          ><img src="@/assets/homepage/ntcicon.png" alt="文大"
        /></a>
        <a class="col-6" href="https://www.codedriven.org/"
          ><img src="@/assets/homepage/codedrivenicon.png" alt="程式驅動"
        /></a>
      </div>
    </div>
  </div>
  <div id="server">
    <div class="container p-5 pt-0">
      <div class="d-flex flex-column justify-content-center">
        <div class="text-center mb-5 fs-1 fw-bold">伺服器狀態</div>
        <a href="https://minecraft-mp.com/server-s303741" target="_blank"
          ><img :src="leaderboard" class="w-100" alt="leaderboard"
        /></a>
      </div>
    </div>
  </div>

  <my-footer></my-footer>
</template>

<script>
import MainNavbar from "@/components/Home/MainNavbar.vue";
import LatestNews from "@/components/Home/LatestNews.vue";
import MyFooter from "../components/MyFooter.vue";
import Navbar from "../components/SubNavbar.vue";

export default {
  name: "HomeView",
  data() {
    return {
      image: require("../assets/minecraftserver.png"),
      leaderboard: "https://minecraft-mp.com/leaderboard-303741-6.png",
    };
  },
  components: {
    MyFooter,
    MainNavbar,
    LatestNews,
    Navbar,
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
section .bg {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("../assets/10950185.jpg");
  background-position: center;
  background-size: cover;
}
section .bg .title {
  letter-spacing: 30px;
  padding-top: 25vh;
}
section .bg .server {
  padding-top: 100px;
}
.introbg1 {
  height: 200px;
  font-size: 1.5rem;
  background-image: url(@/assets/image.png);
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
}
.introbg2 {
  height: 200px;
  font-size: 1.5rem;
  background-image: url(@/assets/image2.png);
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
}
.introbg3 {
  height: 200px;
  font-size: 1.5rem;
  background-image: url(@/assets/image3.png);
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
}


.apppp{
    position: relative;
    width:450px;
    height:450px;
    margin: 0 auto;
}
.product-wrap{
    background:blue;
    position:relative;
    float:left;
    width:150px;
    height:150px;
    margin:0px;
  
}
.product{  
    background:pink;
    position:absolute;
    top:0;
    left:0;
    width:150px;
    height:150px;
    transition: 0.2s;
}
.product0{    
    background:orange;
    position:absolute;
    top:0;
    left:0;
    width:150px;
    height:150px;
    transition: 0.2s;
}
.product1{
  background: url(@/assets/homepage/zombie.png);
  background-size: contain;
}
.product3 p{
  text-align:center;
  display: flex; /* ★ */
  
  align-items: center;
}
.product6{
  background: green;
  background: url(@/assets/homepage/castle.png);
  background-size: contain;
}
.product8{
  background: url(@/assets/homepage/group.png);
  background-size: contain;
}

.product-wrap:hover .product1{
    z-index:100;
    width: 450px;
    height:450px;
  top:0px;
    background: grey;
    background: url(@/assets/homepage/zombie.png);
    background-size: contain;
}
.product-wrap:hover .product2{
    z-index:100;
    width: 450px;
    height:450px;
  top:0px;
  left:-150px;
    background: green;
}
.product-wrap:hover .product3{
    z-index:100;
    width: 450px;
    height:450px;
  top:0px;
  left:-300px;
    background: grey;
}
.product-wrap:hover .product4{
    z-index:100;
    width: 450px;
    height:450px;
  top:-150px;
    background: green;
}
.product-wrap:hover .product5{
    z-index:100;
    width: 450px;
    height:450px;
  top:-50px;
    background: grey;
}
.product-wrap:hover .product6{
    z-index:100;
    width: 450px;
    height:450px;
  top:-150px;
  left:-300px;
    background: green;
    background: url(@/assets/homepage/castle.png);
    background-size: contain;
}
.product-wrap:hover .product7{
    z-index:100;
    width: 450px;
    height:450px;
  top:-300px;
    background: grey;
}
.product-wrap:hover .product8{
    z-index:100;
    width: 450px;
    height:450px;
  top:-300px;
  left:-150px;
    background: green;
    background: url(@/assets/homepage/group.png);
    background-size: contain;
}
.product-wrap:hover .product9{
    z-index:100;
    width: 450px;
    height:450px;
  top:-300px;
  left:-300px;
    background: grey;
}
</style>
