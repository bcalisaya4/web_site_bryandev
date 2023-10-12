<script setup>


</script>
<template>
    <div>
        <section class="home">
            <div class="home-content">
                <h1>Hola, Soy Bryan</h1>
                <h3>Fullstack Developer</h3>
                <p>
                    Soy un desarrollador Fullstack con más de 2 años de experiencia, 
                    durante los cuales he liderado proyectos y capacitado a compañeros 
                    de equipo en tecnologías como Vue.js, Django y Docker.
                </p>
                <div class="btn-box">
                    <a href="#">Acerca de mi</a>
                    <a href="#">Contactame</a> 
                </div>
            </div>
            <span class="home-imgHover">
            </span>
            <!--             
            <div class="home-sci">
                <img
                    style="height: 25px; width:auto" 
                    src="src\assets\images\icons\github-icon.png" 
                    alt="LinkedIn Icon"
                    >
                <img
                    style="height: 20px; width:auto" 
                    src="src\assets\images\icons\linkedin-icon.png" 
                    alt="GitHub Icon"
                    >
            </div> -->

        </section>
    </div>
</template>
<style scope>
.home{
    height: 100vh;
    background: url('/src/assets/images/home-image-2.png') no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    padding: 0 8%;
}
.home-content{
    max-width: 750px;
}
.home-content h1{

    font-size: 5rem;
    font-weight: 700;
}
.home-content h3{
    font-size: 32px;
    font-weight: 700;
    color: #0080b3;
}

.home-content p{
    font-size: 2rem;
    margin: 2rem 0 4rem;
}
.home-content .btn-box{
    display: flex;
    justify-content: space-between;
    width: 345px;
    height: 50px;
}
.btn-box a{
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 150px;
    height: 100%;
    background: #0080b3;
    border: 2px solid #0080b3;
    border-radius: 8px;
    font-size: 19px;
    color: #E0EAF1;
    text-decoration: none;
    font-weight: 600;
    letter-spacing: 1px;
    z-index: 1;
    overflow: hidden;
    transition: 0.5s;
}

.btn-box a:hover{
    color: #0080b3;
}
.btn-box a:nth-child(2){
    background: transparent;
    color: #0080b3;
}
.btn-box a:nth-child(2):hover{
    color: #F0F0F0;
}
.btn-box a:nth-child(2)::before{
    background: #0080b3;
}
.btn-box a::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: #F0F0F0;
    z-index: -1;
    transition: 0.5s;
}

.btn-box a:hover::before{
    width: 100%;
}
/*
.home-sci{
    position: absolute;
    bottom: 40px;
    width: 170px;
    background-color: aquamarine;
}*/

.home-imgHover{
    position: absolute;
    top: 0;
    right: 0;
    width: 45%;
    height: 100%;
    background: transparent;
    /*border: 2px solid red;   */
    transition: 3s;
}
.home-imgHover:hover{
    background: rgb(255, 255, 255);
    opacity: .6;
}

</style>