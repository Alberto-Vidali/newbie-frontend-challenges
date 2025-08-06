<script setup>

    import { ref, onMounted, onUnmounted } from 'vue';

    let mobileMode = ref(0)

    const checkWidth = () => {
        mobileMode.value = window.innerWidth <= 375 ? 1 : 0
    }

    // Viene eseguita all'avvio del programma
    onMounted(() => {
        checkWidth()
        window.addEventListener('resize', checkWidth)
    })

    // Rimuove l'event listener se il componente viene smontato
    onUnmounted(() => {
        window.removeEventListener('resize', checkWidth)
    })
    
</script>

<template>
    <body class="min-h-screen flex flex-col justify-between items-center m-auto bg-purple-200 relative">
        <div>

        </div>
        <header class="absolute top-0">
            <img src="/background-pattern-mobile.svg" alt="" v-if="mobileMode == 1">
            <img src="/background-pattern-desktop.svg" alt="" v-if="mobileMode == 0">
        </header>
        <main class="z-10 absolute top-[10%]">
            <slot/>
        </main>
        <footer>
            <div class="attribution">
                Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
                Coded by <a href="#">Hazerin</a>.
            </div>
        </footer>
    </body>
</template>

<style scoped>
    
</style>