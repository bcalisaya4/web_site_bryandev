<script setup>
import {ref} from 'vue';
const openNav = () => {
    mobileMenu.value.width= '100%'
}
const closeNav = () => {
    console.log("9.9")
    mobileMenu.value.width= '0%'
}
//function closeNav() {
//  console.log("Este es un mensaje de comprobacion EXIT")
//}
const mobileMenu = ref({
    width: '0%',
})
</script>
<template>
    <div>
        <div class="container_header">
            <div class="logo">
                <!--img src="src\assets\images\logo_perfil.png" alt="logo de la marca"-->
            </div>
            <div class="sections-page">
                <nav>
                    <ul class="nav-links">
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Experience</a></li>
                        <li><a href="#">About</a></li>
                        <!-- <li><a href="#">Otros</a></li> -->
                    </ul>
                </nav>
                <!--a href="#" class="btn"><button>Contact</button></a-->

                <a @click="openNav()" class="menu"><button>&#8801;</button></a>
            </div>
            <div class="overlay" :style="mobileMenu">
                <a @click="closeNav()" class="close">&times;</a>
                <div class="overlay-content">
                    <a href="#">Service</a>
                    <a href="#">Projects</a>
                    <a href="#">About</a>
                    <a href="#">About</a>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Nunito', sans-serif;
    font-size: 20px;
}
body{
    background-color: #F0F0F0;
}
.container_header{
    width: 100%;
    position: absolute;
    z-index: 5;
    background-color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 85px;
    padding: 5px 10%;
    box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);
}
.container_header .logo{
    cursor: pointer;
}
.container_header .logo img{
    height: 80px;
    width: auto;
}
.container_header .logo img:hover{
    transform: scale(1.2);
}

.container_header .sections-page{
    width: 40%;
    display: flex;
    justify-content: space-between;
}
.container_header .nav-links{
    list-style: none;
}
.container_header .nav-links li{
    display: inline-block;
    padding: 0 20px;
}
.container_header .nav-links li:hover{
    transform: scale(1.2);
}
.container_header .nav-links a{
    font-size: 700;
    color: #333333;
    text-decoration: none;
}
.container_header .nav-links a:hover{
    font-size: 700;
    color: #3498DB;
}

.container_header .btn button,
    .container_header .menu button{
    font-weight: 700;
    padding: 9px 25px;
    background-color: black;
    color: white;
    border:none;
    border-radius: 50px;
    cursor: pointer;
    transition: all 0.3s ease 0s;

}
.container_header .btn button:hover{
    background: #5DADE2;
    color:  #000000;
    transform: scale(1.1);
}
@media screen and (max-width: 800px) {
    .nav-links, .btn{
        display: none;
    }
    .menu{
        display: inherit;
    }
    
}

/*Nav*/

.container_header a{
    text-decoration: none;
}
.container_header .overlay{
    height: 100%;
    width: 0;
    position: fixed;
    z-index: 10;
    left: 0;
    top: 0;
    background-color: #F0F0F0;
    overflow: hidden;
    transition: all 0.3s ease 0s;
}

.container_header .overlay .overlay-content{
    display: flex;
    height: 100%;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.container_header .overlay a{
    padding: 15px;
    font-size: 56px;
    font-weight: 700;
    display: block;
    transition: all 0.3s ease 0s;
    font-weight: 700;
    color: #333333;
}
.header .overlay a:hover,
.header .overlay a:focus{
    color: #0080b3;
}
.header .overlay .close{
    position: absolute;
    top: 20px;
    right: 45px;
    font-size: 65px;
}
@media screen and (max-height:450px) {
    .container_header .overlay a{
        font-size: 20px;
    }
    .header .overlay .close{
        font-size: 40px;
        top: 15px;
        right: 35px;
    }
}


</style>
