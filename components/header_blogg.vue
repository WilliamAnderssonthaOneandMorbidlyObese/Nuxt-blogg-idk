<template>
    <div class="text-[#FFF500] flex justify-between">
        <div>
        
        <div class="flex ">
            <input type="checkbox" id="drawer-toggle" class="relative hidden peer">

            <label for="drawer-toggle" class="p-4 flex flex-col peer-checked:opacity-0 peer-checked:rotate-180 duration-500">
                <div class="w-9 h-[2px] m-1 bg-[#FFF500] rounded-sm"></div>
                <div class="w-9 h-[2px] m-1 bg-[#FFF500] rounded-sm"></div>
                <div class="w-9 h-[2px] m-1 bg-[#FFF500] rounded-sm"></div>  
            </label>

            <div class="fixed w-72 h-screen transition-all duration-500 transform -translate-x-full bg-black/90 peer-checked:translate-x-0">
               
                <div class="px-6 py-4">
                    <label for="drawer-toggle" class="p-4 transition-all flex justify-between items-center">
                        <div class="text-lg">BLOGG CONTENT</div>
                        <div class="">
                            <div class="w-6 h-[2px] -rotate-45 bg-[#FFF500] rounded-sm absolute"></div>
                            <div class="w-6 h-[2px] rotate-45 bg-[#FFF500] rounded-sm absolute"></div>
                        </div> 
                    </label>
                  
                    <div class="flex flex-col">

                    </div>
                </div>
              </div>
          </div>
     </div>
     <div class="w-24">
        <NuxtLink to="/"><logo_home></logo_home></NuxtLink>
     </div>
        <div>
        about us
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>