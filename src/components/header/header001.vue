<template>
    <div class="container_header">
        <div class="logo">
            <!--img src="src\assets\images\logo_perfil.png" alt="logo de la marca"-->
        </div>
        <nav>
            <ul class="nav-links">
                <li><a href="#">Service</a></li>
                <li><a href="#">Projects</a></li>
                <li><a href="#">sobre mods</a></li>
                <!-- <li><a href="#">Otros</a></li> -->
            </ul>
        </nav>
        <a href="#" class="btn"><button>Contact</button></a>
    </div>
</template>
<style scoped>
*{
    font-size: 20px;
}
.container_header{
 background-color: rgb(0, 35, 36);
 display: flex;
 justify-content: space-between;
 align-items: center;
 height: 90px;
 padding: 5px 10%;
}
.container_header .logo{
    cursor: pointer;
}
.container_header .logo img{
    height: 85px;
    width: auto;
}
.container_header .logo:hover{
    transform: scale(1.3);
    transition: all 0.4s;
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
    color: aliceblue;
    text-decoration: none;
}
.container_header .nav-links li a:hover{
    color:blueviolet
}
.container_header .btn button{
    font-weight: 700;
    color: rgb(35, 9, 83);
    padding: 9px 25px;
    background-color: aliceblue;
    border:none;
    border-radius: 50px;
    cursor: pointer;
}

.container_header .btn button:hover{
    background-color: whitesmoke;
    color:blueviolet;
    transform: scale(1.2);
}
</style>