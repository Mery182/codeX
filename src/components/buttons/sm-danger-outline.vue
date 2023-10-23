<script setup>

// import TheIconChevron from '../components/icons/TheIconChevron.vue';
</script>

<template>
    <button class="secondary-outline">
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
    --squircle-smooth: 0.8;
    --squircle-radius: 20px;
    color: rgba(var(--color-danger), 1);
    border: 1px solid rgba(var(--color-bg-secondary), .7);
}

.secondary-outline {
    background-color: rgba(var(--color-signal), .0);
    border: 1px solid rgba(var(--color-danger), .2);

}

.secondary-outline:hover {
    background-color: rgba(var(--color-danger), .2);


}

.secondary-outline:disabled {
    color: rgba(var(--color-line), 1);
    border: 1px solid rgba(var(--color-line), 1);
    background-color: rgba(var(--color-line), .0);
}
</style>