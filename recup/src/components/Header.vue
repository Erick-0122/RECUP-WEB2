<template>

    <header class="header">
        <div class="top-bar">
            <div class="logo">
                <img src="/logo.png" alt="Logo">
            </div>

            <div class="search-container">
            <input
            type="text"
            placeholder="Buscar produtos, marcas e muito mais..."
            />

            <button>
                <i class="fas fa-search"></i>
            </button>
        </div>
        </div>

        <div class="bottom-bar">
            <nav class="cep-menu">
                <a href="#" class="fas fa-location-dot"></a>
                <a href="#">Informe o seu <strong>CEP</strong></a>
            </nav>
            <nav class="left-menu">
                <a href="#">Categorias</a>
                <a href="#">Ofertas</a>
                <a href="#">Cupons</a>
                <a href="#">Supermercado</a>
                <a href="#">Moda</a>
                <a href="#"class="mercado-play">
                    <span class="gratis">GRÁTIS</span>
                    Mercado Play
                </a>
                <a href="#">Vender</a>
                <a href="#">Contato</a>
            </nav>

            <nav class="right-menu">
                <a href="#">Crie sua conta</a>
                <a href="#">Entre</a>
                <a href="#">Compras</a>
                <a href="#" class="fas fa-shopping-cart"></a>
            </nav>
        </div>
    </header>

</template>

<style scoped>
    .header {
    background: #ffe600;
    padding: 12px 60px;
    border-bottom: 2px solid black;
    }

    .top-bar {
    display: flex;
    align-items: center;
    gap: 30px;
    }

    .logo img {
    height: 40px;
    padding-right: 20px;
    }

    .search-container {
    width: 600px;
    display: flex;
    background: white;
    border-radius: 2px;
    overflow: hidden;
    box-shadow: 0 1px 2px rgba(0,0,0,.15);
    }

    .search-container input {
    flex: 1;
    border: none;
    padding: 14px;
    font-size: 16px;
    outline: none;
    }

    .search-container button {
    border: none;
    position: relative;
    background: white;
    width: 60px;
    cursor: pointer;
    font-size: 18px;
    }

    .search-container button::before {
        content: "";
        position: absolute;
        left: 0;
        top: 20%;      /* distância do topo */
        height: 60%;   /* altura da linha */
        width: 1px;
        background: #e6e6e6;
    }

    .bottom-bar {
    margin-top: 12px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    }
    .mercado-play {
    position: relative;
    text-decoration: none;
    color: black;
    }

    .gratis {
        position: absolute;
        top: -10px;
        left: 20px;

        background: #00a650;
        color: white;

        font-size: 9px;
        font-weight: bold;

        padding: 1px 4px;
        border-radius: 8px;

        text-transform: uppercase;
    }

    .cep-menu a{
    display: flex;
    text-decoration: none;
    color: rgba(0,0,0,.75);
    gap: 8px;
    }
    
    .left-menu,
    .right-menu {
    display: flex;
    gap: 20px;
    }

    .left-menu a,
    .right-menu a {
    text-decoration: none;
    color: rgba(0,0,0,.75);
    font-size: 14px;
    }

    .left-menu a:hover,
    .right-menu a:hover {
    color: rgba(0,0,0,1);
    }
</style>