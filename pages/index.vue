<template>
    <div class="bg-fixed bg-cover flex items-center justify-center  bg-left-top w-full h-screen " style="background-image: url('/background-1.jpg');">
        <div class=" bg-black/50 w-11/12 h-[98%] m-8 rounded-lg ">
            <div class=" text-[#FFF500] font-medium text-lg">
               
            </div>
            <div>

            </div>
    
        </div>
        
    </div>
</template>

<script setup>

const { data } = await useAsyncData('page-data',() => queryContent('/markdown/polish_m.md').findOne())

</script>


<style scoped>

</style>