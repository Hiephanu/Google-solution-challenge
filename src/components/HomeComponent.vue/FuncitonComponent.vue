<template>
    <section class="bg-black text-center">
        <div>
            <div class="h-24">
                <p>.</p>
                <h1 class="text-white text-center text-[30px] mt-12">
                    Explore the world
                </h1>
                <h2 class="text-white text-center mt-12">
                    Easy to search about many animal around the world
                </h2>
            </div>
            <div class="grid grid-cols-3 mt-36 gap-4 ml-4 mr-4">
                <div v-for="(Animal,index) in AnimalArr" :key="index">
                    <div class="relative">
                        <img :src="Animal.path" alt="">
                        <h1 class="absolute top-[10px] text-white">{{ Animal.title }}</h1>
                    </div>
                </div>
            </div>
            <button class="bg-white pl-5 pr-5 pt-3 pb-3 rounded inline-block mt-10">
                Search
            </button>
        </div>
    </section>
</template>
<script>
    import { ref } from 'vue';
    export default{
     setup(){
            const AnimalArr=ref([
                {
                    path:'https://images01.nicepage.com/c461c07a441a5d220e8feb1a/112beb4aa06c5a758acac4da/123.jpg',
                    title:'It is the image of fish in the sea'
                },
                {
                    path:'https://images01.nicepage.com/c461c07a441a5d220e8feb1a/88b584008438593693841927/3f8d3833-72b3-3072-3d51-57dad152da82.jpg',
                    title:'It is monkey '
                },
                {
                    path:'https://images01.nicepage.com/c461c07a441a5d220e8feb1a/15b282e9ca1c5228a1cfbb6c/4a1d4947-fd02-e665-4d57-deac20b3eb39.jpg',
                    title:'It is Komordo'
                }
            ])
            return {
                AnimalArr
            }
        }
    }
</script>