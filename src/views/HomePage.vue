<template>
    <div class="header h-screen">
        <NavBar/>
        <HeaderComponent class="mt-32"/>
    </div>
    <div class="bg-black">
        <FuncitonComponent/>
        <AboutUs/>
        <FooterComponent/>
    </div>
</template>
<script>
    import NavBar from '@/components/HomeComponent.vue/NavBar.vue';
    import HeaderComponent from '@/components/HomeComponent.vue/HeaderComponent.vue';
    import FuncitonComponent from '@/components/HomeComponent.vue/FuncitonComponent.vue';
    import AboutUs from '@/components/HomeComponent.vue/AboutUs.vue';
    import FooterComponent from '@/components/HomeComponent.vue/FooterCompinent.vue';
    export default{
        components:{
            NavBar,
            HeaderComponent,
            FuncitonComponent,
            AboutUs,
            FooterComponent
        }
    }
</script>
<style scoped>
.header{
    background-image: url('https://images01.nicepage.com/c461c07a441a5d220e8feb1a/6c43943bbf88586fa1937f43/Untitled1min.jpg');
}
</style>