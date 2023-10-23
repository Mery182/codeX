<script setup>

// import TheIconChevron from '../components/icons/TheIconChevron.vue';
</script>

<template>
    <button class="primary">
        <slot></slot>
    </button>
</template>

<style scoped>
button {
    display: flex;
    align-items: center;
    margin: 10px 10px;
    letter-spacing: 0.2px;
    height: 28px;
    border-radius: 8px;
    outline: none;
    border: none;
    --squircle-smooth: 0.8;
    --squircle-radius: 20px;
    color: var(--c-white);
}

.primary {
    /* background-color: var(--color-signal); */
    background-color: rgba(var(--color-signal), 1);
}

.primary:hover {
    background-color: var(--color-signal-hover);
}

.primary:disabled {
    color: rgba(var(--color-text-contrast-low), 1);
    background-color: rgba(var(--color-bg-secondary), .7);
}
</style>