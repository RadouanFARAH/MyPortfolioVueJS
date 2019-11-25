<template>
	<dir id="Header">
  <nav>
   
    <router-link to="/"><img src="../assets/img/logo.png" class="logo"></router-link>   
    
    <router-link to="/Contact" class="items">Contact</router-link> 
    <router-link to="/Projects" class="items">Projects</router-link>
    <router-link to="/Skills" class="items">Skills</router-link>
    <router-link to="/Me" class="items">About Me</router-link>
   
  </nav>

  </dir>


  
</template>


<style lang="scss">
     
     #Header nav {
       width: 95%;
       color: rgb(175, 166, 166);
       min-height: 50px;
       font-family:comfortaa;

     }
     

     #Header .logo {
    
      float: left;
      height: 80px;
      border-radius: 50%;
      border: black 2px dotted
      
     }

    

     #Header .items{
       border: black 2px;
       
       padding: 1px;
      margin-top: 1.4em;
      float: right;
      margin-left: 15px;
      outline: none;
      font-size: 15px;
      font-weight: 600;
      color:black;
      text-decoration: none;

            &:hover {
             outline: none;
             color: #ff4d5a;
             text-decoration: none;
                 }
            &:focus {
             outline: none;
             color: #ff4d5a;
             text-decoration: none;
                 }
                 
                 &:actived {
             outline: none;
             color: #ff4d5a;
             text-decoration: none;
                 }     


     }


     

</style>


 