<script setup>
    import { faqs } from '../utils';
    import { ref } from 'vue';

    // Numero in array dei valori per il v-for
    for (let faq in faqs) {
        console.log(faq)
    }

    // Accesso ai valori di domande e risposte
    console.log(faqs[0].faq[0].question)

    const buttonPressed = ref([0,0,0,0])
    
</script>

<template>
    <section class="flex flex-col gap-4" v-for="faqIdx in Object.keys(faqs)">
        <hr v-if="faqIdx != 0">
        <div class="flex items-center justify-between gap-2 text-nowrap">
            <h2 class=" max-w-[75%] font-bold hover:text-purple-600 cursor-pointer" @click="() => {
                if (buttonPressed[faqIdx] == 0) {
                buttonPressed[faqIdx] = 1
            } 
            else {
                buttonPressed[faqIdx] = 0
            }
            }">
                {{ faqs[faqIdx].faq[0].question }}
            </h2>
            <button @click="() => buttonPressed[faqIdx] = 1" class="w-[30px] aspect-[1/1] cursor-pointer" v-if="buttonPressed[faqIdx] == 0">
                <img class="w-full" src="/icon-plus.svg" alt="plus">
            </button>
            <button @click="() => buttonPressed[faqIdx] = 0" class="w-[30px] aspect-[1/1] cursor-pointer" v-if="buttonPressed[faqIdx] == 1">
                <img class="w-full" src="/icon-minus.svg" alt="plus">
            </button>
        </div>
        <p v-if="buttonPressed[faqIdx] == 1">
            {{  faqs[faqIdx].faq[0].answer }}
        </p>
    </section>
</template>

<style scoped>

</style>