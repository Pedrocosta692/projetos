<template>
    <header>
        <nav class="container">
            <a class="navbar-brand " href="#">Star Wars Universe</a>
            <form class="d-flex">
                <input class="form-control me-2" type="search" placeholder="Pesquisar Personagens" aria-label="Search">
            </form>
        </nav>
    </header>
</template>

<script>
export default{
    name:'BarraNavegacao'
}
</script>

<style scoped>

    header{
        background-color: var(--color-background-nav);
        width: 100%;
        height: 80px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    nav{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    a{
        width: 346px;
        height: 42px;
        left: 169px;
        top: 18px;
        font-style: normal;
        font-weight: 600;
        font-size: 32px;
        line-height: 42px;
    }


    input{
        
        width: 288px;
        height: 29px;
        left: 983px;
        top: 27px;
        background: #ffffff;
        border-radius: 4px;
        padding-left: 110px;
    }

</style>