<template>
    <div class="bg-fixed bg-cover flex justify-center  bg-left-top min-h-screen" style="background-image: url('/background-3.jpg');">
    
        <div class="text-[#FFF500] font-medium text-lg flex flex-col lg:w-4/6 z-50">
            <div class="bg-black/70 p-4 rounded-lg m-8">
             <ContentRenderer :value = "data[4]">
                 <ContentRendererMarkdown :value = "data[4]"></ContentRendererMarkdown>
             </ContentRenderer>
            </div>            
        </div>

    </div>
</template>

<script setup>

const { data } = await useAsyncData('page-data', () => queryContent('/markdown/').find())

</script>

<style scoped>
:deep(){
    color: #FFF500;
}
:deep(h1) { font-size: 35px; margin-top: 15px; margin-bottom: 15px; font-weight: bold; }
:deep(h2) { font-size: 30px; margin-top: 30px; margin-bottom: 15px; font-weight: semibold; } 
:deep(p) { margin-top:15px; } 
:deep(h3){ margin-top: 7px; margin-bottom: 7px; } 
:deep(h4) { font-size: 35px; margin-top: 15px; margin-bottom: 15px; font-weight: bold; }
:deep(ul) { list-style-type: disc; margin-top: 7px; margin-bottom: 7px; padding-left: 15px; } :deep(strong) { font-weight: bold; } 
:deep(em){ font-style: italic; } 

</style>