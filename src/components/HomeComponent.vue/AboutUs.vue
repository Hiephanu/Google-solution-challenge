<template>
    <section>
        <h1 class="text-white text-center text-[4rem] mt-12">Meeting our product team</h1>
        <div class="grid grid-cols-4 mt-12">
            <div v-for="(Member,index) in TeamArr" :key="index" class="w-48 m-auto">
                    <h1 class="text-center text-white">{{ Member.name }}</h1>
                    <img class="mt-4" :src="Member.path" alt="">
                    <h1 class="text-center text-white mt-4">{{ Member.position }}</h1>
            </div>
        </div>
    </section>
</template>
<script>
import {ref} from 'vue'
    export default{
        setup(){
            const TeamArr=ref([
                {
                    name:'Đoàn Văn Hiệp',
                    path:'https://st.quantrimang.com/photos/image/2021/05/21/AVT-Doi2-1.jpg',
                    position:'FrontEnd Developer'
                },
                {
                    name:'Nam Anh',
                    path:'https://st.quantrimang.com/photos/image/2021/05/21/AVT-Doi2-3.jpg',
                    position:'FrontEnd Developer'
                },
                {
                    name:'Ngọc Anh',
                    path:'https://st.quantrimang.com/photos/image/2021/05/21/AVT-Doi3-1.jpg',
                    position:'Backend Developer'
                },
                {
                    name:'Hiền An',
                    path:'https://st.quantrimang.com/photos/image/2021/05/21/AVT-Doi3-2.jpg',
                    position:'BackEnd Developer'
                },
            ])
            return{
                TeamArr
            }
        }
    }
</script>