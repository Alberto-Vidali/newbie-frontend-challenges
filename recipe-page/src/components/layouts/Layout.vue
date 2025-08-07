<script setup>
  
</script>

<template>
    <section class="min-h-screen flex flex-col justify-between sm:bg-amber-100">
        <main class="flex justify-center sm:my-20">
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
        font-size: 15px; text-align: center;
    }
    .attribution a { 
        color: hsl(228, 45%, 44%); 
    }
</style>
