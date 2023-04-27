<template>
    <div>
        <p>blogg inlägg {{ id }}</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params
</script>

<style scoped>

</style>