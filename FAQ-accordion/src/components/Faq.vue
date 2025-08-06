<script setup>
    import { faqs } from '../utils';

    // Numero in array dei valori per il v-for
    for (let faq in faqs) {
        console.log(faq)
    }

    // Accesso ai valori di domande e risposte
    console.log(faqs[0].faq[0].question)

    const buttonPressed = [0,0,0,0]
    
</script>

<template>
    <section class="flex flex-col gap-4" v-for="faqIdx in Object.keys(faqs)">
        <hr v-if="faqIdx != 0">
        <div class="flex items-center justify-between gap-2">
            <h2 class=" max-w-[75%]">
                {{ faqs[faqIdx].faq[0].question }}
            </h2>
            <button class="w-[30px] aspect-[1/1]">
                <img class="w-full" src="/icon-plus.svg" alt="plus">
            </button>
        </div>
        <p>
            {{  faqs[faqIdx].faq[0].answer }}
        </p>
    </section>
</template>

<style scoped>

</style>