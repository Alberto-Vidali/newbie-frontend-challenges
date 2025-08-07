<script setup>

</script>

<template>
    <section class="min-h-screen bg-gray-200 flex flex-col items-center justify-between">
        <header>
            
        </header>
        <main class="bg-white mx-5 max-w-[335px] sm:max-w-fit sm:mx-auto sm:w-[900px] h-[575px] sm:h-[322px] rounded-2xl">
            <slot/>
        </main>
        <footer>
            <div class="attribution">
                Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
                Coded by <a href="#">Hazerin</a>.
            </div>
        </footer>
    </section>
</template>

<style scoped>
    .attribution { 
        font-size: 15px; 
        text-align: center; 
    }
    .attribution a { 
        color: hsl(228, 45%, 44%); 
    }
</style>
