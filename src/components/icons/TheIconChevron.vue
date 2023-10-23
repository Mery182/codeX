<script setup>
import { IconBrackets } from '@codexteam/icons';

console.log(IconBrackets);

</script>

<template>
    <div class="icon-chevron">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M9 8L5 12L9 16" />
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M15 8L19 12L15 16" />
        </svg>
    </div>
</template>

<style scoped>
.icon-chevron {
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    align-content: center;
    transform: rotate(90deg);
}

.icon-chevron:first-child {
    margin-top: 0px;
}

.icon-chevron:nth-child(2) {
    margin-bottom: 0px;
}
</style>