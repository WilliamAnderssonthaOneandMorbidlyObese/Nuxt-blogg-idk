<template>
    <div class="bg-fixed bg-cover flex items-center justify-center bg-left-top w-full min-h-screen " style="background-image: url('/background-2.jpg');">
        
        <div class=" w-11/12 h-[98%]  ">
            
            <div class="text-[#FFF500] font-medium text-lg flex flex-col lg:grid lg:grid-cols-2">
                <div v-for="d in data" class="bg-black/70 p-4 rounded-lg m-8">
                    <ContentRenderer :value = "d">
                        <ContentRendererMarkdown :value = "d" ></ContentRendererMarkdown>
                    </ContentRenderer>
                </div>             
                
            </div>
            
        </div>
        
    </div>
</template>
    
<script setup>
    definePageMeta({
        layout:'blogg'
    })

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
:deep(ul) { list-style-type: disc; margin-top: 7px; margin-bottom: 7px; padding-left: 15px; } 
:deep(strong) { font-weight: bold; } 
:deep(em){ font-style: italic; } 
:deep(img){ width: 100%; height: 20rem; object-fit: cover; margin-top: 15px; margin-bottom: 15px; box-shadow: 2px; border-color: #FFF500; border-width: 2px; }

</style>