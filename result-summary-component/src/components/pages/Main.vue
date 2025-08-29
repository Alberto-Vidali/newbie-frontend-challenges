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
        <div class="">
            <h3>Summary</h3>
            <div class="flex justify-between">
                <div class="flex">
                    <img src="/icon-reaction.svg" alt="icon"><p>Reaction</p>
                </div>
                <div class="flex">
                    <p>80</p><p>/ 100</p>
                </div>
                
            </div>
            
            Memory
            92 / 100

            Verbal
            61 / 100

            Visual
            72 / 100

            <button>
               Continue 
            </button>
        </div>
    </section>
</template>

<style scoped>

</style>