<script setup>
    import Faq from '../Faq.vue';
</script>

<template>
    <section class="w-[300px] xl:w-[550px] bg-white p-4 xl:p-8 rounded-2xl">
        <div class="flex items-center justify-start pb-4 gap-4 text-4xl font-[700]">
            <img class="xl:h-[35px]" src="/icon-star.svg" alt="">
            <h1 class="xl:text-4xl">FAQs</h1>
        </div>
        <div class="flex flex-col gap-4">
            <Faq/>
        </div>
    
    </section>
</template>

<style scoped>

</style>