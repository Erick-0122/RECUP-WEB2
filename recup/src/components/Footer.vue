<script setup lang="ts">
</script>

<template>
  <footer class="footer">
    <div class="footer-links">
      <a href="#">Trabalhe conosco</a>
      <a href="#">Termos e condições</a>
      <a href="#">Promoções</a>
      <a href="#">Como cuidamos da sua privacidade</a>
      <a href="#"><i class="fas fa-universal-access"></i>Acessibilidade</a>
      <a href="#">Contato</a>
      <a href="#">Informações sobre seguros</a>
      <a href="#">Programa de Afiliados</a>
    </div>

    <div class="footer-info">
      <p>Copyright © 1999-2026 Ebazar.com.br LTDA.</p>

      <p>
        CNPJ n.º 03.007.331/0001-41 /
        Av. das Nações Unidas, nº 3.003,
        Bonfim, Osasco/SP - CEP 06233-903 -
        empresa do grupo Mercado Livre.
      </p>
    </div>
  </footer>
</template>

<style scoped>
    .footer {
        background: #ffffff;
        border-top: 1px solid #e6e6e6;
        padding: 20px 0;
    }

    .footer-links {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 24px;

        margin-bottom: 12px;
    }

    .footer-links a {
        text-decoration: none;
        color: #333;
        font-size: 14px;
    }

    .footer-links a:hover {
        color: #3483fa;
    }

    .footer-info {
        text-align: center;
    }

    .footer-info p {
        color: #999;
        font-size: 12px;
        margin: 4px 0;
    }
</style>