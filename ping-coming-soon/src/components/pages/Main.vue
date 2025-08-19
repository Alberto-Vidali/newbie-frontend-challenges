<script setup>

</script>

<template>
    <section class="h-[1000px] flex flex-col items-center justify-between p-5">
        <div class="flex flex-col items-center justify-around gap-10">
            <img src="/logo.svg" alt="">
            <div class="flex flex-col items-center">
                <h2 class="text-[30px] text-gray-400">
                    We are launching <strong class="text-black">soon!</strong>
                </h2>
                <p>
                    Subscribe and get notified
                </p>
            </div>
            <div class="flex flex-col w-full gap-5">
                <div class="h-10 w-full rounded-full flex items-center justify-start border-1 border-gray-400">
                    <input class="px-5 w-full focus-within:border-none" type="text" placeholder="Your email address...">
                </div>
                <div class="bg-blue-500 h-10 w-full rounded-full flex items-center justify-center">
                    <button class="text-white">Notify Me</button>
                </div>
            </div>
            <img src="/illustration-dashboard.png" alt="">
        </div>
        <div class="flex flex-col justify-center items-center h-[10%] gap-5">
            <div class="flex justify-center gap-2">
                <button class="text-2xl border-blue-400 border-1 rounded-full h-10 aspect-[1/1] text-blue-400">
                    <i class="fa-brands fa-facebook-f"></i>
                </button>
                <button class="text-2xl border-blue-400 border-1 rounded-full h-10 aspect-[1/1] text-blue-400">
                    <i class="fa-brands fa-twitter"></i>
                </button>
                <button class="text-2xl border-blue-400 border-1 rounded-full h-10 aspect-[1/1] text-blue-400">
                    <i class="fa-brands fa-instagram"></i>
                </button>
            </div>
            <p class="text-[14px] text-gray-400">&copy; Copyright Ping. All rights reserved.</p>
        </div>
    </section>
</template>

<style scoped>

</style>