<template>

    <nav class="navbar navbar-expand-md navbar-light navbar-laravel">
        <div class="container">

            <router-link class='navbar-brand' :to="{ name: 'home'}">Home</router-link>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <!-- Left Side Of Navbar -->
                <ul class="navbar-nav mr-auto">

                </ul>

                <!-- Right Side Of Navbar -->
                <ul class="navbar-nav ml-auto">
                    <!-- Authentication Links -->

                    
                    
                    <li>
                        <router-link class='nav-link' :to="{ name: 'login'}">Login</router-link>
                    </li>
                    <li>
                        <router-link class='nav-link' :to="{ name: 'register'}">Register</router-link>
                    </li>
                    <li>
                        <router-link class='nav-link' :to="{ name: 'me'}">Dashboard</router-link>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

</template>
<script>
 
  export default{
   

   created(){
        console.log('Hit From Nav');
      }
    
  }
</script>