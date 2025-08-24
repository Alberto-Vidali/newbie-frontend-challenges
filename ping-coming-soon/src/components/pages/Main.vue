<script setup>
import { computed, ref } from 'vue';

    const emailIsValid = ref(0)
    let hello = ref("")

    function emailCheck() {
        emailIsValid.value = 0;
        
        for (let i = 0; i < hello.value.length; i++) {
            console.log(hello.value[i])
            if (hello.value[i] == "@" && emailIsValid.value == 0) {
                emailIsValid.value = 1
                console.log(emailIsValid.value)
            } else if (hello.value[i] == "@" && emailIsValid.value == 1) {
                emailIsValid.value = 2;
                console.log(emailIsValid.value)
            }
        }
        if (emailIsValid.value == 0) emailIsValid.value = 2
        hello.value = "";
    }
</script>

<template>
    <section class="h-[1000px] flex flex-col items-center justify-between p-5 sm:w-4xl">
        <div class="flex flex-col items-center justify-around gap-10">
            <img src="/logo.svg" alt="">
            <div class="flex flex-col items-center sm:gap-2">
                <h2 class="text-[30px] sm:text-4xl text-gray-400">
                    We are launching <strong class="text-black">soon!</strong>
                </h2>
                <p class="sm:text-xl">
                    Subscribe and get notified
                </p>
            </div>
            <div class="flex flex-col sm:flex-row w-full gap-5">
                <div v-if="emailIsValid == 0" class="h-10 w-full rounded-full flex items-center justify-start border-1 border-gray-400">
                    <input v-model="hello" id="email-box" class="px-5 w-full focus-within:border-none focus-within:outline-none" type="text" placeholder="Your email address...">
                </div>
                <div v-if="emailIsValid == 1" class="h-10 w-full rounded-full flex items-center justify-start border-1 border-gray-400">
                    <input v-model="hello" id="email-box" class="px-5 w-full focus-within:border-none focus-within:outline-none text-green-400 focus-within:text-black" type="text" placeholder="We sent a confirmation email. Thanks!">
                </div>
                <div v-if="emailIsValid == 2" class="h-10 w-full rounded-full flex items-center justify-start border-1 border-gray-400">
                    <input v-model="hello" id="email-box" class="px-5 w-full focus-within:border-none focus-within:outline-none text-red-400 focus-within:text-black" type="text" placeholder="This email address is not valid.">
                </div>

                <div class="bg-blue-500 h-10 w-full rounded-full flex items-center justify-center sm:w-[30%]">
                    <button @click="emailCheck()" id="email-button" class="text-white w-full">Notify Me</button>
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