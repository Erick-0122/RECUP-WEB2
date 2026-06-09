<script setup lang="ts">
    import BackgroundContent from './Background-content.vue'
</script>

<template>
    <section class="hero">
        <BackgroundContent />
    </section>
    
</template>

<style scoped>
    .hero {
        
        min-height: 600px;
        background: linear-gradient(
            180deg,
            #ffe600 50%,
            #ffe539 60%,
            #fff4bf 80%,
            #f5f5f5 100%
        );
    }
    

</style>