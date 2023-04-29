<template>
    <div class="text-[#FFF500] flex justify-between items-center">
        <div>
        
        <div class="flex h-full ">
                <input type="checkbox" id="drawer-toggle" class="relative hidden peer">
                
                <label for="drawer-toggle" class="py-8 pl-4 flex flex-col peer-checked:opacity-0 peer-checked:rotate-180 duration-500">
                    <div class="w-12 h-[2px] m-1 bg-[#FFF500] rounded-sm"></div>
                    <div class="w-12 h-[2px] m-1 bg-[#FFF500] rounded-sm"></div>
                    <div class="w-12 h-[2px] m-1 bg-[#FFF500] rounded-sm"></div>  
                </label>
                
                <div class="fixed w-72 h-full transition-all duration-500 transform -translate-x-full bg-[#FFF500] peer-checked:translate-x-0">
                    
                <div class="px-6 py-4">
                    <label for="drawer-toggle" class="p-6 transition-all flex justify-between items-center border-b-[1px] border-black">
                        <div class="text-xl text-black">Blogg Content</div>
                        <div>
                            <div class="w-6 h-[2px] -rotate-45 bg-black rounded-sm absolute"></div>
                            <div class="w-6 h-[2px] rotate-45 bg-black rounded-sm absolute"></div>
                        </div> 
                    </label>
                  
                    <div class="flex flex-col text-lg text-black">
                        <ul>
                            <li class="p-6 underline underline-offset-4">
                                <NuxtLink to="/blogg#polish-modernism">Polish Modernism</NuxtLink>
                            </li>
                            <li class="p-6 underline underline-offset-4">
                                <NuxtLink to="/blogg#historical-context">Historical Context</NuxtLink>
                            </li>
                            <li class="p-6 underline underline-offset-4">
                                <NuxtLink to="/blogg#why-art-matters">Why Art Matters</NuxtLink>
                            </li>
                            <li class="p-6 underline underline-offset-4">
                                <NuxtLink to="/blogg#the-importance-of-art-intentions">Art Intentions</NuxtLink>
                            </li>
                        </ul>

                    </div>
                </div>
              </div>
          </div>
     </div>
     <div class="w-40">
        <NuxtLink to="/"><logo_home></logo_home></NuxtLink>
     </div>
        <div class="p-6 text-xl font-medium">
       <NuxtLink to="/about">ABOUT US</NuxtLink>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>