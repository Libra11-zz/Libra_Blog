<template>
   <div class="wrap">
   <div class="section-title wow fadeInUp">
     <h1>My Skills</h1>
     <span class="border"></span>
   </div>
   <article class="row">
     <ul>
       <li class="html">
         <em>HTML/HTML5</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
       <li class="css">
         <em>CSS/CSS3</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
       <li class="php">
         <em>PHP/OOP</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
       <li class="mysql">
         <em>MYSQL</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
     </ul>
   </article>
   <article class="row">
     <ul>
       <li class="jquery">
         <em>JQUERY</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
       <li class="javascript">
         <em>JAVASCRIPT</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
       <li class="seo">
         <em>SEO</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
       <li class="unix">
         <em>UNIX</em>
         <div>
           <span class="animated fadeInLeft"></span>
         </div>
       </li>
     </ul>
   </article>
 </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="less" scoped>
@import './index';
body { 
  background: #111c27; 
  font: 14px/1.6 "Open Sans",Helvetica,Arial,sans-serif; 
  color: #697279;}
.wrap{
  max-width: 960px;
  margin: 0 auto;
  position: relative;
  padding: 0 20px;
}
.section-title h1{
    margin: 0;
    line-height: 50px;
    letter-spacing: 5px;
    font-weight: 600;
    color: white;
}.border{
  display: block;
  height: 10px;
  margin-bottom: 40px;
  width: 100px;
  background: #ED5565;
}
.row{
  width: 50%;
  min-height: 1px;
  float: left;
  position: relative;
  display: inline-block;
}.row ul {
  margin: 0 20px 0 0 !important;
  text-align: left !important;
  padding: 0;
}.row ul li{
  list-style: none !important;
  
}.row ul li em{
  display: block;
  margin-bottom: 15px;
}.row ul li div{
  margin-bottom: 35px;
  border-radius: 3px 3px 3px 3px;
  -webkit-border-radius: 3px 3px 3px 3px;
  background: #09131B;
  height: 42px;
  overflow: hidden;
}.row ul li div span{
  height: 42px;
  width: 50%;
  display: block;
  border-radius: 3px 3px 3px 3px;
  -webkit-border-radius: 3px 3px 3px 3px;
}
.row ul li.html div span { background: #E13C4C; width: 90%; }
.row ul li.css div span { background: #ffdb43; width: 90%; }
.row ul li.php div span { background: #9D2027; width: 80%; }
.row ul li.mysql div span { background: #3498db; width: 75%; }
.row ul li.jquery div span { background: #2ecc71; width: 60%; }
.row ul li.javascript div span { background: #A94034 }
.row ul li.seo div span { background: #FF8137; width: 60%; }
.row ul li.unix div span { width: 65%; background: #0CBFB3; }

.animated {
  -webkit-animation-duration: 1s;
  animation-duration: 1s;
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
}.fadeInLeft {
  -webkit-animation-name: fadeInLeft;
  animation-name: fadeInLeft;
}
@-webkit-keyframes fadeInLeft {
  0% {
    opacity: 0;
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }100% {
    opacity: 1;
    -webkit-transform: none;
    transform: none;
  }
}
@keyframes fadeInLeft {
  0% {
    opacity: 0;
    -webkit-transform: translate3d(-100%, 0, 0);
    -ms-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }100% {
    opacity: 1;
    -webkit-transform: none;
    -ms-transform: none;
    transform: none;
  }
}

</style>