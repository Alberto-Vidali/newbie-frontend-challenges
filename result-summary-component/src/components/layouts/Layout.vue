<script setup>
    
</script>

<template>
    <header class="hidden">

    </header>
    <main class="flex flex-col justify-center flex-1">
        <slot/>
    </main>
    <footer>
        <div class="attribution">
            Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
            Coded by <a href="#">Alberto Vidali</a>.
        </div>
    </footer>
</template>

<style scoped>
    .attribution { font-size: 13px; text-align: center; }
    .attribution a { color: hsl(228, 45%, 44%); }
</style>