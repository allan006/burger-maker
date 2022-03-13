<template>
    <nav id="nav">
        <RouterLink to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </RouterLink>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/pedidos">Pedidos</RouterLink>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
    props: ["logo", "alt" ]
}
</script>

<style scoped>
    #nav{
        background-color: #222;
        border-bottom: #111;
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    #nav #logo-url{
        margin: auto;
        margin-left: 0px;
    }
    
    #logo{
        height: 40px;
        width: 40px;
    }

    #nav a {
        color: #FCBA03;
        text-decoration: none;
        margin: 12px;
        transition: .5s;
    }

    #nav a:hover {
        color: #FFF;
    }
</style>