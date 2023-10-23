<script setup>

// import TheIconChevron from '../components/icons/TheIconChevron.vue';
</script>

<template>
    <button class="danger">
        <slot></slot>
    </button>
</template>

<style scoped>
button {
    display: flex;
    align-items: center;
    margin: 10px 10px;
    letter-spacing: 0.2px;
    height: 36px;
    padding: 0 10px;
    border-radius: 8px;
    outline: none;
    border: none;
    --squircle-smooth: 0.8;
    --squircle-radius: 20px;
    color: var(--c-white);
}

slot {
    padding: 0 10px;
}

.danger {
    background-color: rgba(var(--color-danger), 1);
}

.danger:hover {
    background-color: var(--color-danger-hover);
}

.danger:disabled {
    color: rgba(var(--color-text-contrast-low), 1);
    background-color: rgba(var(--color-bg-secondary), .7);
}
</style>