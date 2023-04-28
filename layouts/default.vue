<template>
    <div>
        <header class=" overflow-hidden bg-black">
            <header_logo></header_logo>
            <div class="flex justify-around  text-[#FFF500] font-normal text-base pb-4 mt-3 ">
                <ul class="flex justify-around w-full lg:mx-12 lg:justify-center">
                    <li class="rounded-md px-4 p-2 border-2 border-transparent hover:border-[#FFF500]"><NuxtLink to="/">HOME</NuxtLink></li>
                    
                    
                    <li class="rounded-md px-4 p-2 border-2 border-transparent hover:border-[#FFF500]"><NuxtLink to="/blogg">BLOGG</NuxtLink></li>
                    
                    <li class="rounded-md px-4 p-2 hidden sm:block border-2 border-transparent hover:border-[#FFF500]"> <NuxtLink to="<--!3d design-->">3D-Engineer</NuxtLink> </li>
                    <li class="rounded-md px-8 block sm:hidden p-2 border-2 border-transparent hover:border-[#FFF500]"> <NuxtLink to="<--!3d design-->">3D</NuxtLink> </li>
                    
                    <li class="rounded-md px-4 p-2 border-2 border-transparent hover:border-[#FFF500]"><NuxtLink to="/about">ABOUT US</NuxtLink></li>
                </ul>        
            </div>
        </header>
        
        <div>
            <slot/>
        </div>

        <footer class=" overflow-hidden bg-black p-4">
            <div class="text-[#FFF500]/90 flex justify-between ">
                <div class="flex justify-start items-start">

                    <ul class="mx-8">
                        <li>
                            2023
                        </li>
                    </ul>
                    <ul>
                        <li>
                            Copyright ©
                        </li>
                    </ul>
                    <ul class="mx-2">
                        <li>
                            Good Entertainment
                        </li>
                        <li>
                            Studio INC.
                        </li>
                    </ul>
                    <ul class="mx-6 hidden sm:block">
                    <li>
                        Created:
                    </li>
                    <li>
                        William Andersson
                    </li>
                   </ul>
                   <ul class= "mx-6 hidden md:block">
                    <li>
                        Design: Władysław
                    </li>
                    <li>
                        Starobrzański
                    </li>
                    </ul>
                </div>
                
                <LogoHome class="hidden lg:block w-32 ml-40"></LogoHome>
            </div>            
        </footer>
    </div> 
</template>

<script setup>


</script>

<style scoped>

   li .router-link-exact-active {
            text-decoration: underline;
        }


</style>