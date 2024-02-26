<script lang="ts">
console.log("This is the home page")
import MathMenu from '@/components/MathMenu.vue';
export default { components: { MathMenu } }
</script>

<template>
    <MathMenu/>
</template>

<style scoped>
    h1 {
        color: black;
    }
    .homepage {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
</style>