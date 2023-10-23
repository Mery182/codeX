<script setup>

// import TheIconChevron from '../components/icons/TheIconChevron.vue';
</script>

<template>
    <button class="primary-outline">
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
    --squircle-smooth: 0.8;
    --squircle-radius: 20px;
    color: rgba(var(--color-signal), 1);
    border: 1px solid rgba(var(--color-signal), .4);
}

.primary-outline {
    background-color: rgba(var(--color-signal), .0);
    border: 1px solid rgba(var(--color-signal), .4);

}

.primary-outline:hover {
    background-color: rgba(var(--color-signal), .12);


}

.primary-outline:disabled {
    color: rgba(var(--color-text-contrast-low), 1);
    background-color: rgba(var(--color-bg-secondary), .7);
}
</style>