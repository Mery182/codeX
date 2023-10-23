<script setup>

// import TheIconChevron from '../components/icons/TheIconChevron.vue';
</script>

<template>
    <button class="primary-ghost">
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

}

.primary-ghost {
    background-color: rgba(var(--color-signal), .0);
    outline: none;
    border: none;

}

.primary-ghost:hover {
    background-color: rgba(var(--color-signal), .12);


}

.primary-ghost:disabled {
    color: rgba(var(--color-line), 1);
    border: 1px solid rgba(var(--color-line), 0);
    background-color: rgba(var(--color-line), .0);
}
</style>