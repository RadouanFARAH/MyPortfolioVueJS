<template>

	<div class="projects-container">


		<div class="projects-content">

<!------------------------------------------------------------------------------------------------- -->
			<div class="header">
			  <div class="fadeInDown animated">	
				<button :class="{'active-btn': (projects==1)}" @click="projects=1">
					<i class="fas fa-desktop" style="font-size: 23px;"></i>
                    <p style="font-size: 15px; font-family:comfortaa;">WEB</p>
				</button>
				<button :class="{'active-btn': (projects==2)}" @click="projects=2">
					<i class="fas fa-mobile" style="font-size: 23px;"></i>
                    <p style="font-size: 15px;font-family:comfortaa;">MOBILE</p>
				</button>
				
			   </div>
			</div>

<!------------------------------------------------------------------------------------------------- -->

		   <!-- WEB -->


			<div class="container " v-if="projects==1">

               <div class="row">  

				 
				<!------------------------------------------------------------------------------------------------ - --> 	
                   <dir class="col-sm-12 col-md-6 col-lg-4 col-xl-4 zoomIn animated">
                    
                             <div class="card-cover ">

                                   <p style="font-size: 17px;font-family:comfortaa;">My Store Application</p>
                                  <img class="A" src="../assets/img/mystore.png" alt="">
                                  <img class="B" src="../assets/img/mystore-hover.png" alt="">
                                   
                                           
                             </div>                       
                     
                   </dir>
                <!------------------------------------------------------------------------------------------------- -->
                   <dir class="col-sm-12 col-md-6 col-lg-4 col-xl-4 zoomIn animated">
                    
                             <div class="card-cover ">
                             	    <p style="font-size: 17px;font-family:comfortaa;">My Hotel Application</p>
                                  <img class="A" src="../assets/img/myroom.png" alt="">
                                  <img class="B" src="../assets/img/myroom-hover.png" alt=""> 

                                       
                             </div>                       
                     
                   </dir>

                <!------------------------------------------------------------------------------------------------- -->
              
                   <dir class="col-sm-12 col-md-6 col-lg-4 col-xl-4 zoomIn animated">
                    
                             <div class="card-cover ">

                             	    <p style="font-size: 17px;font-family:comfortaa;"> My Notes Application</p>
                                  <img class="A" src="../assets/img/mynote.png" alt=""> 
                                  <img class="B" src="../assets/img/mynote-hover.png" alt=""> 

                                  
                             </div>                       
                     
                   </dir>
          	    

               </div>
			</div>

<!------------------------------------------------------------------------------------------------ - -->

			<!-- MOBILE -->
			<div class="container " v-if="projects==2">

               <div  style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%);" class="row">  

                <!------------------------------------------------------------------------------------------------- -->
                   <dir  class=" zoomIn animated">
                    
                             <div class="card-cover ">

                             	    <p style="font-size: 17px;font-family:comfortaa;">In The Middle Of Building Mobile Apps</p>
                                  <img src="../assets/img/Building.jpg" alt=""> 
                                           
                             </div>                       
                     
                   </dir>


                
          	    

               </div>
			</div>

<!------------------------------------------------------------------------------------------------- -->			



		</div>


	</div>
</template>



<style lang="scss">
.projects-container {
  width: 100%;

  a {
    color: #fff;
    text-decoration: none;
  }
}

.projects-content {
  
  
  box-sizing: border-box;
  
  width: 100%;
  margin: auto;
}

.header {
  
  text-align: center; 
  margin-left: 50%;
  transform: translate(-50%);
  margin-bottom: 30px;


  button {
    background-color: transparent;
      
      text-align: center;
      border:none;
      cursor: pointer;
      outline: none;
      font-size: 20px;
      
      margin-left: 0px;
      color: #474747;  
  }

  .active-btn {
    background-color: transparent;
      
      text-align: center;
      border:none;
      cursor: pointer;
      outline: none;
      
      
      margin-left: 0px;
      color: #ff4d5a; 
  }
}





.card-cover {
	
     
     text-align: center;
     margin-bottom: 20px;
    box-shadow: 0 0 10px 2px #606060;
    background-color: #fff;
  
  img {
    width: 100%;
    height: auto;
        
  }
  .B{
      display: none;
    }
}

.card-cover:hover {
  
  
       .A{
        display: none;
       }
       .B{
        display: block;
       }
  
 
}

.mobile-cover {
  
     
     text-align: center;
     margin-bottom: 20px;
  
  img {
    
    height: 200px;
    width: auto;

    
  }
}

.active-btn {
  background: royalblue;
  transition: all 0.2s;
}



@media (max-width: 1069px) {
  .projects-content {
    padding-top: 90px;
  }
}

@media (max-width: 460px) {
  .projects-content {
    width: 100%;
    padding-right:0;
    padding-left:0;



    .header{
      padding: 0 20px;
      box-sizing: border-box;
    }
  }
}
</style>



<script>

import  { mapActions } from 'vuex'

export default {
  name: "projects",
  data() {
    return {
      projects: 1,
      
    }
  },

  methods : {
    ...mapActions({
      openModal : 'openModalAction',
    }),
  }
}
</script>
