<template>
    <div>
        <header class=" overflow-hidden bg-black border-b-2 border-[#FFF500]">
            <header_blogg></header_blogg>
        </header>
        <div>
            <slot/>
        </div>
        <footer class="overflow-hidden bg-black p-4 border-t-2 border-[#FFF500]">
            <ref_footer></ref_footer>
        </footer>
   </div>
</template>

<script setup>

</script>

<style scoped>

</style>