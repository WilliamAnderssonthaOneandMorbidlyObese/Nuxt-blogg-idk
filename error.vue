<template>
    <div class="h-screen w-screen bg-black flex justify-center">
        <div class="m-10 w-1/2 h-1/2 bg-[#FFF500] flex flex-col items-center shadow-md shadow-[#FFF500]">
            <div class="text-7xl font-bold m-8">error : {{ error.statusCode }}</div>
            <div class="text-3xl">ojoj...inte bra</div>
            <div class="text-3xl">{{ error.message }}</div>
            <div class="text-center w-1/4 m-8">                                                          
                <img src="error_page.png">                                                                                             
            </div>
        </div>
    </div>
</template>

<script setup>
    defineProps(['error'])
</script>

<style scoped>

</style>