<template>
    <Transition name="fade">
        <div id="lg">
            <div v-if="show" class="preloader">

                <TheLogo />

            </div>
        </div>
    </Transition>
</template>

<script>

import TheLogo from "../components/TheLogo.vue"

export default {
    components: {
        TheLogo
    },
    data() {
        return {
            show: true,
            open: false


        }
    },
    computed: {

    },
    mounted() {
        this.open = true;
        this.showToggle()

    },
    methods: {
        showToggle() {
            setTimeout(() => {
                this.open = true;
                this.show = false;

            }, 1500);
        },

    },

}
</script>

<style scoped></style>