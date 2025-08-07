<script setup>
  
</script>

<template>
    <section class="max-w-[500px] bg-white rounded-2xl">
        <img class="rounded-t-2xl" src="/image-omelette.jpeg" alt="omelette">
        <div class="flex flex-col p-8 gap-4 text-[15px] tracking-wide">
            <h1 class="text-4xl font-bold text-red-900">
                Simple Omelette Recipe
            </h1>
    
            <p>
                An easy and quick dish, perfect for any meal. This classic omelette combines beaten eggs cooked 
                to perfection, optionally filled with your choice of cheese, vegetables, or meats.
            </p>
    
            <div class="flex flex-col gap-4 bg-red-50 p-4 pr-14">
                <h2 class="text-2xl text-red-900 font-bold">
                    Preparation time
                </h2>
                <!--Tailwind di default rimuove i puntini, da reinserire e applicare lo stile-->
                <ul role="list" class="list-disc marker:text-md pl-4 flex flex-col gap-2 relative">
                    <li><span class="relative left-2"><strong>Total:</strong> Approximately 10 minutes</span></li>
                    <li><span class="relative left-2"><strong>Preparation:</strong> 5 minutes</span></li>
                    <li><span class="relative left-2"><strong>Cooking:</strong> 5 minutes</span></li>
                </ul>
            </div>

            <div class="flex flex-col gap-4 p-4">
                <h2 class="text-2xl text-red-900 font-bold">
                    Ingredients
                </h2>
                <!--Tailwind di default rimuove i puntini, da reinserire e applicare lo stile-->
                <ul role="list" class="list-disc marker:text-md pl-4 flex flex-col gap-2 relative">
                    <!--Lo span serve a permettere di posizionare il testo più o meno lontano dai puntini-->
                    <li><span class="relative left-2">2-3 large eggs</span></li>
                    <li><span class="relative left-2">Salt, to taste</span></li>
                    <li><span class="relative left-2">Pepper, to taste</span></li>
                    <li><span class="relative left-2">1 tablespoon of butter or oil</span></li>
                    <li><span class="relative left-2">Optional fillings: cheese, diced vegetables, cooked meats, herbs</span></li>
                </ul>
            </div>

            <hr class="text-gray-400">

            <div class="flex flex-col gap-4 p-4">
                <h2 class="text-2xl text-red-900 font-bold">
                    Instructions
                </h2>
                <!--Tailwind di default rimuove i puntini, da reinserire e applicare lo stile-->
                <ol role="list" class="list-decimal marker:text-md marker:font-bold pl-4 flex flex-col gap-2 relative">
                    <!--Lo span serve a permettere di posizionare il testo più o meno lontano dai puntini-->
                    <li><span class="relative left-2"><strong>Beat the eggs: </strong>In a bowl, beat the eggs with a pinch of salt and pepper until they are well mixed. 
            You can add a tablespoon of water or milk for a fluffier texture.</span></li>
                    <li><span class="relative left-2"><strong>Heat the pan: </strong>Place a non-stick frying pan over medium heat and add butter or oil.</span></li>
                    <li><span class="relative left-2"><strong>Cook the omelette: </strong>Once the butter is melted and bubbling, pour in the eggs. Tilt the pan to ensure 
            the eggs evenly coat the surface.</span></li>
                    <li><span class="relative left-2"><strong>Add fillings (optional): </strong>When the eggs begin to set at the edges but are still slightly runny in the 
            middle, sprinkle your chosen fillings over one half of the omelette.</span></li>
                    <li><span class="relative left-2"><strong>Enjoy: </strong>Serve hot, with additional salt and pepper if needed.</span></li>
                </ol>
            </div>

            <hr class="text-gray-400">

            <div class="flex flex-col gap-4 pr-2">
                <h2 class="text-2xl text-red-900 font-bold">
                    Nutrition
                </h2>
                <p>The table below shows nutritional values per serving without the additional fillings.</p>
                <div class="flex flex-col gap-2">
                    <div class="flex justify-between px-4">
                        <p>
                            Calories
                        </p>
                        <h3 class="font-bold text-red-800">
                            277kcal
                        </h3>
                    </div>
                    <hr class="text-gray-400">
                    <div class="flex justify-between px-4">
                        <p>
                            Carbs
                        </p>
                        <h3 class="font-bold text-red-800">
                            0g
                        </h3>
                    </div>
                    <hr class="text-gray-400">
                    <div class="flex justify-between px-4">
                        <p>
                            Protein
                        </p>
                        <h3 class="font-bold text-red-800">
                            20g
                        </h3>
                    </div>
                    <hr class="text-gray-400">
                    <div class="flex justify-between px-4">
                        <p>
                            Fat
                        </p>
                        <h3 class="font-bold text-red-800">
                            22g
                        </h3>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>

</style>
