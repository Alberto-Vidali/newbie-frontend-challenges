<script setup>

    import { ref, onMounted, onUnmounted } from 'vue';

    const shareSocial = ref(0)

</script>

<template>
    <!--Da usare l'inherit per far si che i div più interni abbiano un riferimento se uso le percentuali-->
    <section class="h-[inherit] overflow-hidden">
        <div class="h-[38.5%] overflow-hidden">
            <img class="w-fit overflow-hidden" src="/drawers.jpg" alt="">
        </div>

        <div class="flex flex-col justify-between items-center h-[61.5%] p-8 gap-0">
            <h1 class="font-semibold text-lg">
                Shift the overall look and feel by adding these wonderful 
                touches to furniture in your home
            </h1>
    
            <p class="text-[15px] pb-6 tracking-tight">
                Ever been in a room and felt like something was missing? Perhaps 
                it felt slightly bare and uninviting. I’ve got some simple tips 
                to help you make any room feel complete.
            </p>
    
    
            <div class="flex justify-around items-center gap-4 w-full" v-if="shareSocial == 0">
                <div class="flex gap-4 w-full">
                    <img class="w-[40px] aspect-[1/1] rounded-full" src="/avatar-michelle.jpg" alt="">
                    <div>
                        <h2 class="font-semibold">
                            Michelle Appleton
                        </h2>
                        <p class="text-gray-400">
                            28 Jun 2020
                        </p>
                    </div>
                </div>
                <button class="bg-gray-200 w-[40px] aspect-[1/1] flex flex-col justify-center items-center rounded-full">
                    <img class="w-[50%]" src="/icon-share.svg" alt="Share">
                </button>
            </div>
            <div v-if="shareSocial == 0">

            </div>
        </div>
    </section>
</template>

<style scoped>
  
</style>
