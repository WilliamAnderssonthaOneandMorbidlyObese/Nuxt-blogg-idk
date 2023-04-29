<template>
    <div>
        <header class=" overflow-hidden bg-black">
            <header_logo></header_logo>
            <div class="flex justify-around  text-[#FFF500] font-normal text-base pb-4 mt-3 ">
                <ul class="flex justify-around w-full lg:mx-12 lg:justify-center">
                    <li class="rounded-md px-4 p-2 border-[1px] border-transparent hover:border-[#FFF500]"><NuxtLink to="/">HOME</NuxtLink></li>
                    
                    
                    <li class="rounded-md px-4 p-2 border-[1px] border-transparent hover:border-[#FFF500]"><NuxtLink to="/blogg">BLOGG</NuxtLink></li>
                    
                    <li class="rounded-md px-4 p-2 hidden sm:block border-[1px] border-transparent hover:border-[#FFF500]"> <NuxtLink to="<--!3d design-->">3D-Engineer</NuxtLink> </li>
                    <li class="rounded-md px-8 block sm:hidden p-2 border-[1px] border-transparent hover:border-[#FFF500]"> <NuxtLink to="<--!3d design-->">3D</NuxtLink> </li>
                    
                    <li class="rounded-md px-4 p-2 border-[1px] border-transparent hover:border-[#FFF500]"><NuxtLink to="/about">ABOUT US</NuxtLink></li>
                </ul>        
            </div>
        </header>
        
        <div>
            <slot/>
        </div>

        <footer class=" overflow-hidden bg-black p-4 border-t-2 border-[#FFF500]">
            <ref_footer></ref_footer>
        </footer>
    </div> 
</template>

<script setup>


</script>

<style scoped>

   li .router-link-exact-active {
            text-decoration: underline;
            text-underline-offset: 4px ;
        }


</style>