<script setup>

</script>

<template>
    <body class="min-h-screen flex flex-col justify-between items-center m-auto bg-purple-200 relative">
        <div>

        </div>
        <header class="absolute top-0">
            <img src="/background-pattern-mobile.svg" alt="">
        </header>
        <main class="z-10 flex justify-between items-center">
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