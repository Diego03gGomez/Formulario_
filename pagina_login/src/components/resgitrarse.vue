<template lang="">
    <div>
       <header>
<div class="cont_header">
<h1><img src="https://themes.pixelstrap.net/mega_bot/assets/images/logo.svg" alt=""></h1>


</div>


<div class="contenedor_registro">
    <div class="titulo_login">
    
    <h2>Welcome to <span>Megabot!</span></h2>

</div>
    <div class="links">
<a  v-on:click="mostrar_login()"   href="#">Login</a>
<a  v-on:click="mostrar_sing()"     href="#">Signup</a>
</div>



<div id="login" >
  



<div class="cont_campos">
<h3>Email ID</h3>
<i class="fa-solid fa-envelope correo "></i><input class="email" type="email" placeholder="Enter your mail id">

<h3>Password</h3>
<i class="fa-solid fa-lock candado "></i><input class="password" type="password" placeholder="Enter your password">
</div>
<div class="cont_olvido">
    <a href="#">Forgot Password?</a>

</div>



<div class="cont_logear">
    <button>Log me in</button>
</div>

<div class="cont_explicacion">
    <h3>Don t have an account ? <a href="#">Sign up</a></h3>
    
    <h3>or sign in with</h3>

</div>



<div class="cont_continuar">
    
    <a><img src="https://themes.pixelstrap.net/mega_bot/assets/svg/google.svg" alt="">Continue with google</a>
<a><img src="https://themes.pixelstrap.net/mega_bot/assets/svg/apple.svg" alt="">Continue with apple</a>
</div>





</div>


<div id="signup" class="ocultar"  >

<div class="cont_campos2">

<div class="campo">
    <h2>Name</h2>
    <i class="fa-solid fa-user user"></i>
<input type="text" placeholder="Enter your name">
</div>

<div class="campo">
    <h2>Email ID</h2>
    <i class="fa-solid fa-envelope email2"></i>
<input type="text" placeholder="Enter your mail id">
</div>

<div class="campo">
    <h2>Password</h2>
    <i class="fa-solid fa-lock candado1"></i>
<input type="text" placeholder="Enter your passwords">
</div>

<div class="campo">
    <h2>Confirm Password</h2>
    <i class="fa-solid fa-lock candado2"></i>
<input type="text" placeholder="Enter your password">
</div>












</div>

<div class="cont_sign">
    <button>Sign up</button>
</div>

<div class="des2">
    <h4>Already have an account <a href="#">Sign in</a></h4>
</div>







</div>






    






</div>




       </header>
    </div>
</template>
<script>
export default {
    methods: {
        mostrar_sing() {
            let sign = document.querySelector("#signup");
            let login = document.querySelector("#login");
            
            sign.classList.add("mostrar");
            sign.classList.remove("ocultar");
            login.classList.add("ocultar");
            login.classList.remove("mostrar");
        },
        mostrar_login() {
            let sign = document.querySelector("#signup");
            let login = document.querySelector("#login");

            login.classList.add("mostrar");
            login.classList.remove("ocultar");
            sign.classList.add("ocultar");
            sign.classList.remove("mostrar");
        }
    
},
   
}
</script>
<style>
    
</style>