<script setup>

    import { ref, onMounted, onUnmounted } from 'vue';

    // 1 è per mostrare i social della versione mobile, 2 per mostrare quelli del desktop
    const shareSocial = ref(0)

    function toggleShare() {
        if (window.innerWidth <= 640) {
            shareSocial.value == 0 ? shareSocial.value = 1 : shareSocial.value = 0
            console.log(shareSocial.value)
        } else if (shareSocial.value == 0) {
            shareSocial.value == 0 ? shareSocial.value = 2 : shareSocial.value = 0
            console.log(shareSocial.value)
        } else {
            shareSocial.value = 0
            console.log(shareSocial.value)
        }
    }

</script>

<template>
    <!--Da usare l'inherit per far si che i div più interni abbiano un riferimento se uso le percentuali-->
    <section class="h-[inherit] sm:flex">
        <div class="h-[38.5%] sm:h-full sm:w-full overflow-hidden sm:overflow-visible">
            <img class="w-fit sm:h-[100%] rounded-2xl sm:rounded-r-none" src="/drawers.jpg" alt="">
        </div>

        <div class="flex flex-col justify-between items-center h-[61.5%] sm:h-full sm:pt-4">
            <h1 class="font-semibold text-lg sm:text-xl pt-8 sm:pt-3 px-8  tracking-wide">
                Shift the overall look and feel by adding these wonderful 
                touches to furniture in your home
            </h1>
    
            <p class="text-[15px] pb-6 sm:pb-0 tracking-tight px-8  pr-4">
                Ever been in a room and felt like something was missing? Perhaps 
                it felt slightly bare and uninviting. I’ve got some simple tips 
                to help you make any room feel complete.
            </p>
    
    
            <div class="flex justify-around items-center gap-4 w-full px-8 pb-4 " v-if="shareSocial == 0 || shareSocial == 2">
                <div class="flex gap-4 w-full sm:pb-3">
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
                <button @click="() => toggleShare()" class="bg-gray-200 w-[35px] aspect-[1/1] flex flex-col justify-center items-center rounded-full hover:cursor-pointer relative">
                    <img class="w-[50%]" src="/icon-share.svg" alt="Share">
                    <div class="absolute bg-gray-700 rounded-xl p-3 px-8 pr-24 top-[-80px] balloon" v-if="shareSocial == 2">
                        <div class="flex items-center justify-start gap-4">
                            <h2 class="text-gray-400 tracking-[5px]">
                                SHARE
                            </h2>
                            <img src="/icon-facebook.svg" alt="">
                            <img src="/icon-twitter.svg" alt="">
                            <img src="/icon-pinterest.svg" alt="">
                        </div>
                    </div>
                </button>
                
            </div>
            <div class="flex items-center justify-around bg-gray-600 w-full h-[64px] rounded-b-2xl" v-if="shareSocial == 1">
                <div class="flex items-center justify-start gap-4">
                <h2 class="text-gray-400 tracking-[5px]">
                    SHARE
                </h2>
                    <img src="/icon-facebook.svg" alt="">
                    <img src="/icon-twitter.svg" alt="">
                    <img src="/icon-pinterest.svg" alt="">
                </div>
                <button @click="() => toggleShare()" class="bg-white w-[30px] aspect-[1/1] flex flex-col justify-center items-center rounded-full hover:cursor-pointer">
                    <img class="w-[50%] text-white" src="/icon-share.svg" alt="Share">
                </button>
            </div>
        </div>
    </section>
</template>

<style scoped>
    
</style>