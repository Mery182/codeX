<script setup>

// import TheIconChevron from '../components/icons/TheIconChevron.vue';
</script>

<template>
    <button class="secondary-ghost">
        <slot></slot>
    </button>
</template>

<style scoped>
button {
    display: flex;
    align-items: center;
    margin: 10px 10px;
    letter-spacing: 0.2px;
    height: 44px;
    padding: 0 15px;
    border-radius: 8px;
    outline: none;
    --squircle-smooth: 0.8;
    --squircle-radius: 20px;
    color: rgba(var(--color-text-contrast-high-soft), .7);

}

.secondary-ghost {
    background-color: rgba(var(--color-bg-secondary), .0);
    outline: none;
    border: none;


}

.secondary-ghost:hover {
    background-color: rgba(var(--color-bg-secondary), .5);


}

.secondary-ghost:disabled {
    color: rgba(var(--color-line), 1);
    border: 1px solid rgba(var(--color-line), 0);
    background-color: rgba(var(--color-line), .0);
}
</style>