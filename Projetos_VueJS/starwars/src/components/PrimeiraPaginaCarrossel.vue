<template>
    <div class="max-width">
            <h2 class="title">Filmes</h2>
            <div class="carousel owl-carousel">
                <div class="card">
                    <div class="box">
                        <img src="./assets/episode_1.jpg" alt="">
                        <div class="text">Paulo</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="box">
                        <img src="./assets/episode_2.webp" alt="">
                        <div class="text">Julio</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="box">
                        <img src="./assets/episode_3.jpg" alt="">
                        <div class="text">Evelyn</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="box">
                        <img src="./assets/episode_4.webp" alt="">
                        <div class="text">Lauro</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="box">
                        <img src="./assets/episode_5.jpg" alt="">
                        <div class="text">Silvia</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="box">
                        <img src="./assets/episode_6.jpg" alt="">
                        <div class="text">Silvia</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
            </div>
    </div>
</template>

<script>
    export default{
        name: 'PrimeiraPaginaCarrosel'
    }
    
</script>

<style scoped>

    .max-width{
        display: flex;
        justify-content: space-between;
    }

   .max-width .title::after{
    content: "experiências";
}
.max-width .carousel .card{
    background: rgb(255, 255, 255);
    border-radius: 6px;
    padding: 25px 35px;
    text-align: center;
    overflow: hidden;
    transition: all 0.3s ease;
}
.max-width .carousel .card .box{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    transition: all 0.3s ease;
}
.max-width .carousel .card:hover .box{
    transform: scale(1.05);
}
.max-width .carousel .card .text{
    font-size: 25px;
    font-weight: 500;
    margin: 10px 0 7px 0;
}
.max-width .carousel .card img{
    height: 352px;
    width: 268px;
    object-fit: cover;
    border-radius: 10px 10px 0px 0px;
    transition: all 0.3s ease;
}
.max-width .carousel .card:hover img{
    border-color: #fff;
}


</style>