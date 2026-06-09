<script setup lang="ts">
import { onMounted, ref } from 'vue'
import { API_URL } from '../api/api.urls'
import Cardboxes from './Cardboxes.vue'
interface Usuario {
    picture: {
        large: string
    }
}

const usuarios = ref<Usuario[]>([])


async function carregarUsuario() {
  try {
    const response = await fetch(API_URL.usuarios)
    const data = await response.json()
    console.log(data)
    usuarios.value = data.results
  } catch (error) {
    console.error('Erro ao buscar usuário:', error)
  }
}

onMounted(() => {
    carregarUsuario()
})

</script>

<template>
    <section class="hero-content">

        <div class="banner">
            <button class="arrow left" @click="carregarUsuario">
                <i class="fas fa-chevron-left"></i>
            </button>
            <div class="banner-content">
                <div class="banner-left">
                    <img src="/liquida66.png" alt="Liquida 6.6">
                </div>

                <div class="banner-center">
                    <img
                        v-if="usuarios.length"
                        :src="usuarios[0]?.picture?.large"
                        alt="Usuário"
                    >
                </div>

                <div class="banner-right">
                    <img src="/desconto.png" alt="Desconto">
                </div>
            </div>

            <button class="arrow right" @click="carregarUsuario">
                <i class="fas fa-chevron-right"></i>
            </button>
        </div>
        <div class="cardboxes">
            <Cardboxes />
        </div>
        
    </section>
</template>

<style scoped>
    .banner {
        position: relative;
        height: 350px;
        object-fit: cover;
    }

    .banner-content {
    display: flex;
    align-items: center;
    justify-content: center;

    height: 100%;
    max-width: 1200px;
    margin: 0 auto;

    gap: 40px;
    }

    .banner-left,
    .banner-center,
    .banner-right {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .banner-center img {
        height: 280px;
        object-fit: cover;
        border-radius: 100%;
    }
        

    .arrow {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);

        width: 100px;
        height: 100px;

        border: none;
        border-radius: 50%;

        background: white;
        cursor: pointer;

        box-shadow: 0 2px 8px rgba(0,0,0,.15);

        display: flex;
        align-items: center;
        justify-content: center;
    }

    .left {
        left: -35px;
    }

    .right {
        right: -35px;
    }

    .arrow i {
        font-size: 18px;
        color: #3483fa;
    }
    .arrow:hover {
        box-shadow: 0 4px 12px rgba(0,0,0,.25);
    }
</style>