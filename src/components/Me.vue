<template >
	<div>
        <div class="img-container zoomIn animated">
          <img class="me" src="../assets/img/moi.png" alt="">
        </div>
        <div class="msg-container">
            <h1><span>Hi</span>, I'm Redouane FARAH &#128578;</h1>
            <h3>I'm a Full Stack JavaScript Web Developer, based in Rabat, Morocco. I'm very ambitious when it comes to Development and Programming.</h3>
            <br>
            <br>
            <p class="follow animated fadeInUp" >\Follow me/</p>
            <div class="socialMedia animated fadeInUp">
              <a href="https://github.com/FARAH-Redouane" target="_blank"><i class="fab fa-github"></i></a>
              <a href="https://www.linkedin.com/in/redouanefarah/" target="_blank"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>

        

     
  </div>
</template>





<style lang="scss">
   
@import url("https://use.fontawesome.com/releases/v5.0.13/css/all.css");
.follow {
    font-weight: normal;
    font-family: comfortaa;
    font-size: 25px;

}

 .socialMedia{
  font-size: 30px;
  a {
    color: rgb(0, 0, 0);
    padding: 8px;
  }
  a:hover {
    color: #ff4d5a;
    
  }

 } 



.msg-container{
  position: absolute;
  top: 60%;
  left: 38%;
  transform: translate(-50%, -50%);
  text-align: center;
  width: 500px;

  }
  
.img-container{
    position: absolute;
    top: 40%;
    left: 62%;
    transform: translate(-50%, -50%);
    height: 240px;
    width: 240px;
    margin:0 auto;
    overflow: hidden;
    text-align: center;
    animation-delay: 0.4s;
   }
   
h3{
   
    font-weight: normal;
    animation-name: moveInright;
    animation-duration: 2s;
    
    }

h1{
 
    display: inline-block;
    animation-name: moveInleft;
    animation-duration: 2s;
    font-weight: normal;
    font-family: comfortaa;
    font-size: 30px;

  }
    span{
      color: #ff4d5a;
    }
  


@keyframes homeSkew{
  from{transform: translateY(50px) skewY(20deg);}
  50%{transform: translateY(0) skewY(20deg);}
  to{transform: skewY(0)}
}


@keyframes moveInleft {
  0% {
    opacity: 0;
    transform: translateX(-20px); }
  80% { }
  100% {
    opacity: 1;
    transform: translate(0); } }

@keyframes moveInright {
  0% {
    opacity: 0;
    transform: translateX(20px); }
  80% { }
  100% {
    opacity: 1;
    transform: translate(0); } }  
       
</style>