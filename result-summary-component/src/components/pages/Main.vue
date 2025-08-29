<script setup>
    
</script>

<template>
    <section class="flex flex-col flex-1">
        <div class=" flex flex-col items-center justify-between h-[350px] py-8 px-15 bg-gradient-to-b from-purple-700 to-blue-700 rounded-b-3xl text-white">
            <h2 class="">Your Result</h2>
            <div class="flex flex-col justify-center items-center gap-3 text-center rounded-full bg-blue-700 h-[125px] aspect-[1/1]">
                <h1 class="text-5xl font-bold">76</h1>
                <p class="text-gray-300 text-sm">of 100</p>
            </div>
            <div class="flex flex-col items-center gap-3">
               <h1 class="text-3xl font-semibold">Great</h1>
               <p class="text-sm text-center">You scored higher than 65% of the people who have taken these tests.</p> 
            </div>
            
        </div>
        <div class="flex flex-col px-6 gap-5 pt-5">
            <h3 class="font-bold">Summary</h3>
            <div class="flex justify-between bg-red-50 p-2 rounded-xl">
                <div class="flex gap-2">
                    <img src="/icon-reaction.svg" alt="icon"><p class="text-red-500">Reaction</p>
                </div>
                <div class="flex gap-1">
                    <p class="font-semibold">80</p><p class="text-gray-400">/ 100</p>
                </div>
            </div>
            <div class="flex justify-between bg-yellow-50 p-2 rounded-xl">
                <div class="flex gap-2">
                    <img src="/icon-memory.svg" alt="icon"><p class="text-yellow-500">Memory</p>
                </div>
                <div class="flex gap-1">
                    <p class="font-semibold">92</p><p class="text-gray-400">/ 100</p>
                </div>
            </div>
            <div class="flex justify-between bg-green-50 p-2 rounded-xl">
                <div class="flex gap-2">
                    <img src="/icon-verbal.svg" alt="icon"><p class="text-green-500">Verbal</p>
                </div>
                <div class="flex gap-1">
                    <p class="font-semibold">61</p><p class="text-gray-400">/ 100</p>
                </div>
            </div>
            <div class="flex justify-between bg-blue-50 p-2 rounded-xl">
                <div class="flex gap-2">
                    <img src="/icon-visual.svg" alt="icon"><p class="text-blue-500">Visual</p>
                </div>
                <div class="flex gap-1">
                    <p class="font-semibold">72</p><p class="text-gray-400">/ 100</p>
                </div>
            </div>

            <button class="bg-gray-700 py-3 rounded-3xl text-white">
               Continue 
            </button>
        </div>
    </section>
</template>

<style scoped>

</style>