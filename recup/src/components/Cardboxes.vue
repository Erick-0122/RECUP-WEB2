<script setup lang="ts">
</script>

<template>
    <div class="benefits">
    <div class="card">
        <h3>Frete grátis</h3>

        <img src="/frete.png" alt="Frete grátis">

        <p>Benefício por ser sua primeira compra.</p>

        <button>Mostrar produtos</button>
    </div>

    <div class="card">
        <h3>Entre na sua conta</h3>

        <img src="/conta.png" alt="Conta">

        <p>Aproveite ofertas para comprar tudo que quiser.</p>

        <button>Entrar na sua conta</button>
    </div>

    <div class="card">
        <h3>Insira sua localização</h3>

        <img src="/localizacao.png" alt="Localização">

        <p>Confira os custos e prazos de entrega.</p>

        <button>Informar localização</button>
    </div>

    <div class="card">
        <h3>Meios de Pagamento</h3>

        <img src="/pagamento.png" alt="Localização">

        <p>Pague suas compras com rapidez e segurança</p>

        <button>Mostrar meios</button>
    </div>

    <div class="card">
        <h3>Menos de 100R$</h3>

        <img src="/pobre.png" alt="Localização">

        <p>Confira produtos com preços mais baixos.</p>

        <button>Mostrar produtos</button>
    </div>

        <div class="card">
        <h3>Mais vendidos</h3>

        <img src="/vendidos.png" alt="Localização">

        <p>Explore os produtos que são tendência.</p>

        <button>Ir para mais vendidos</button>
    </div>
    
</div>
</template>

<style scoped>
    .benefits {
        display: flex;
        justify-content: center;
        gap: 16px;
        flex-wrap: wrap;
        
        max-width: 1400px;
        margin: 0 auto;
        padding: 20px;
    }

    .card {
        width: 180px;

        background: #fff;
        border-radius: 8px;

        padding: 16px;

        display: flex;
        flex-direction: column;
        align-items: center;

        text-align: center;

        box-shadow: 0 1px 4px rgba(0,0,0,.12);
    }

    .card h3 {
        width: 100%;
        text-align: left;
        font-size: 22px;
        margin-bottom: 20px;
    }

    .card img {
        width: 100px;
        height: 100px;
        object-fit: contain;
    }

    .card p {
        font-size: 14px;
        color: #666;
        min-height: 60px;
    }

    .card button {
        width: 100%;
        border: none;
        border-radius: 4px;

        padding: 10px;

        background: #eaf2ff;
        color: #3483fa;

        cursor: pointer;
    }
</style>