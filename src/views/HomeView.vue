<script setup>
// import DarkMode from '../components/DarkMode.vue';
import ThePlus from '../components/icons/ThePlus.vue';
import TheIconChevron from '../components/icons/TheIconChevron.vue';
import smPrimary from '../components/buttons/sm-primary.vue';
import smSecondary from '../components/buttons/sm-secondary.vue'
import smDanger from '../components/buttons/sm-danger.vue'
import mdPrimary from '../components/buttons/md-primary.vue';
import mdSecondary from '../components/buttons/md-secondary.vue'
import mdDanger from '../components/buttons/md-danger.vue'
import lgPrimary from '../components/buttons/lg-primary.vue';
import lgSecondary from '../components/buttons/lg-secondary.vue'
import lgDanger from '../components/buttons/lg-danger.vue'
import smPrimaryOutline from '../components/buttons/sm-primary-outline.vue'
import smSecondaryOutline from '../components/buttons/sm-secondary-outline.vue'
import smDangerOutline from '../components/buttons/sm-danger-outline.vue'
import mdPrimaryOutline from '../components/buttons/md-primary-outline.vue'
import mdSecondaryOutline from '../components/buttons/md-secondary-outline.vue'
import mdDangerOutline from '../components/buttons/md-danger-outline.vue'
import lgPrimaryOutline from '../components/buttons/lg-primary-outline.vue'
import lgSecondaryOutline from '../components/buttons/lg-secondary-outline.vue'
import lgDangerOutline from '../components/buttons/lg-danger-outline.vue'
import smSecondaryGhost from '../components/buttons/sm-secondary-ghost.vue'
import smPrimaryGhost from '../components/buttons/sm-primary-ghost.vue'
import smDangerGhost from '../components/buttons/sm-danger-ghost.vue'
import mdPrimaryGhost from '../components/buttons/md-primary-ghost.vue'
import mdSecondaryGhost from '../components/buttons/md-secondary-ghost.vue'
import mdDangerGhost from '../components/buttons/md-danger-ghost.vue'
import lgPrimaryGhost from '../components/buttons/lg-primary-ghost.vue'
import lgSecondaryGhost from '../components/buttons/lg-secondary-ghost.vue'
import lgDangerGhost from '../components/buttons/lg-danger-ghost.vue'
import { useDark, useToggle } from '@vueuse/core'

const isDark = useDark({
    selector: 'body',
    attribute: 'color-scheme',
    valueLight: 'light',
    valueDark: 'dark',
})

const toggleDark = useToggle(isDark)
</script>

<template>
    <div color-scheme="isDark ? 'dark' : 'light'">
        <label class="switch">
            <input @click="toggleDark()" type="checkbox">
            <span class='slider round'></span>
        </label>
        <div class="meprod-container">
            <div class="one-blok-button">
                <div class="blok-button">
                    <smPrimary>Button </smPrimary>
                    <smPrimary>
                        <ThePlus /> Button&ensp;
                    </smPrimary>
                    <smPrimary>
                        &ensp;Button
                        <TheIconChevron />
                    </smPrimary>
                    <smPrimary>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smPrimary>

                    <smPrimary>
                        <ThePlus />
                    </smPrimary>
                </div>
                <div class="blok-button">
                    <smSecondary>Button</smSecondary>
                    <smSecondary>
                        <ThePlus /> Button&ensp;
                    </smSecondary>
                    <smSecondary>
                        &ensp;Button
                        <TheIconChevron />
                    </smSecondary>
                    <smSecondary>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smSecondary>
                    <smSecondary>
                        <ThePlus />
                    </smSecondary>
                </div>
                <div class="blok-button">
                    <smDanger>Button</smDanger>
                    <smDanger>
                        <ThePlus /> Button&ensp;
                    </smDanger>
                    <smDanger>&ensp;Button
                        <TheIconChevron />
                    </smDanger>
                    <smDanger>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smDanger>
                    <smDanger>
                        <ThePlus />
                    </smDanger>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <mdPrimary>Button</mdPrimary>
                    <mdPrimary>
                        <ThePlus /> Button&ensp;
                    </mdPrimary>
                    <mdPrimary>&ensp;Button
                        <TheIconChevron />
                    </mdPrimary>
                    <mdPrimary>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdPrimary>
                    <mdPrimary>
                        <ThePlus />
                    </mdPrimary>
                </div>
                <div class="blok-button">
                    <mdSecondary>Button</mdSecondary>
                    <mdSecondary>
                        <ThePlus /> Button&ensp;
                    </mdSecondary>
                    <mdSecondary> &ensp;Button
                        <TheIconChevron />
                    </mdSecondary>
                    <mdSecondary>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdSecondary>
                    <mdSecondary>
                        <ThePlus />
                    </mdSecondary>
                </div>
                <div class="blok-button">
                    <mdDanger>Button</mdDanger>
                    <mdDanger>
                        <ThePlus /> Button&ensp;
                    </mdDanger>
                    <mdDanger>&ensp;Button
                        <TheIconChevron />
                    </mdDanger>
                    <mdDanger>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdDanger>
                    <mdDanger>
                        <ThePlus />
                    </mdDanger>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <lgPrimary>Button</lgPrimary>
                    <lgPrimary>
                        <ThePlus /> Button&ensp;
                    </lgPrimary>
                    <lgPrimary>&ensp;Button
                        <TheIconChevron />
                    </lgPrimary>
                    <lgPrimary>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgPrimary>
                    <lgPrimary>
                        <ThePlus />
                    </lgPrimary>
                </div>
                <div class="blok-button">
                    <lgSecondary>Button</lgSecondary>
                    <lgSecondary>
                        <ThePlus /> Button&ensp;
                    </lgSecondary>
                    <lgSecondary> &ensp;Button
                        <TheIconChevron />
                    </lgSecondary>
                    <lgSecondary>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgSecondary>
                    <lgSecondary>
                        <ThePlus />
                    </lgSecondary>
                </div>
                <div class="blok-button">
                    <lgDanger>Button</lgDanger>
                    <lgDanger>
                        <ThePlus /> Button&ensp;
                    </lgDanger>
                    <lgDanger>&ensp;Button
                        <TheIconChevron />
                    </lgDanger>
                    <lgDanger>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgDanger>
                    <lgDanger>
                        <ThePlus />
                    </lgDanger>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <smPrimaryOutline>Button</smPrimaryOutline>
                    <smPrimaryOutline>
                        <ThePlus /> Button&ensp;
                    </smPrimaryOutline>
                    <smPrimaryOutline>&ensp;Button
                        <TheIconChevron />
                    </smPrimaryOutline>
                    <smPrimaryOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smPrimaryOutline>
                    <smPrimaryOutline>
                        <ThePlus />
                    </smPrimaryOutline>
                </div>
                <div class="blok-button">
                    <smSecondaryOutline>Button</smSecondaryOutline>
                    <smSecondaryOutline>
                        <ThePlus /> Button&ensp;
                    </smSecondaryOutline>
                    <smSecondaryOutline>&ensp;Button
                        <TheIconChevron />
                    </smSecondaryOutline>
                    <smSecondaryOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smSecondaryOutline>
                    <smSecondaryOutline>
                        <ThePlus />
                    </smSecondaryOutline>
                </div>
                <div class="blok-button">
                    <smDangerOutline>Button</smDangerOutline>
                    <smDangerOutline>
                        <ThePlus /> Button&ensp;
                    </smDangerOutline>
                    <smDangerOutline>&ensp;Button
                        <TheIconChevron />
                    </smDangerOutline>
                    <smDangerOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smDangerOutline>
                    <smDangerOutline>
                        <ThePlus />
                    </smDangerOutline>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <mdPrimaryOutline>Button</mdPrimaryOutline>
                    <mdPrimaryOutline>
                        <ThePlus /> Button&ensp;
                    </mdPrimaryOutline>
                    <mdPrimaryOutline>&ensp;Button
                        <TheIconChevron />
                    </mdPrimaryOutline>
                    <mdPrimaryOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdPrimaryOutline>
                    <mdPrimaryOutline>
                        <ThePlus />
                    </mdPrimaryOutline>
                </div>
                <div class="blok-button">
                    <mdSecondaryOutline>Button</mdSecondaryOutline>
                    <mdSecondaryOutline>
                        <ThePlus /> Button&ensp;
                    </mdSecondaryOutline>
                    <mdSecondaryOutline>&ensp;Button
                        <TheIconChevron />
                    </mdSecondaryOutline>
                    <mdSecondaryOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdSecondaryOutline>
                    <mdSecondaryOutline>
                        <ThePlus />
                    </mdSecondaryOutline>
                </div>
                <div class="blok-button">
                    <mdDangerOutline>Button</mdDangerOutline>
                    <mdDangerOutline>
                        <ThePlus /> Button&ensp;
                    </mdDangerOutline>
                    <mdDangerOutline>&ensp;Button
                        <TheIconChevron />
                    </mdDangerOutline>
                    <mdDangerOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdDangerOutline>
                    <mdDangerOutline>
                        <ThePlus />
                    </mdDangerOutline>
                </div>
            </div>
            <div class="one-block-button">
                <div class="blok-button">
                    <lgPrimaryOutline>Button</lgPrimaryOutline>
                    <lgPrimaryOutline>
                        <ThePlus /> Button&ensp;
                    </lgPrimaryOutline>
                    <lgPrimaryOutline>&ensp;Button
                        <TheIconChevron />
                    </lgPrimaryOutline>
                    <lgPrimaryOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgPrimaryOutline>
                    <lgPrimaryOutline>
                        <ThePlus />
                    </lgPrimaryOutline>
                </div>
                <div class="blok-button">
                    <lgSecondaryOutline>Button</lgSecondaryOutline>
                    <lgSecondaryOutline>
                        <ThePlus /> Button&ensp;
                    </lgSecondaryOutline>
                    <lgSecondaryOutline>&ensp;Button
                        <TheIconChevron />
                    </lgSecondaryOutline>
                    <lgSecondaryOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgSecondaryOutline>
                    <lgSecondaryOutline>
                        <ThePlus />
                    </lgSecondaryOutline>
                </div>
                <div class="blok-button">
                    <lgDangerOutline>Button</lgDangerOutline>
                    <lgDangerOutline>
                        <ThePlus /> Button&ensp;
                    </lgDangerOutline>
                    <lgDangerOutline>&ensp;Button
                        <TheIconChevron />
                    </lgDangerOutline>
                    <lgDangerOutline>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgDangerOutline>
                    <lgDangerOutline>
                        <ThePlus />
                    </lgDangerOutline>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <smPrimaryGhost>Button</smPrimaryGhost>
                    <smPrimaryGhost>
                        <ThePlus /> Button&ensp;
                    </smPrimaryGhost>
                    <smPrimaryGhost>&ensp;Button
                        <TheIconChevron />
                    </smPrimaryGhost>
                    <smPrimaryGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smPrimaryGhost>
                    <smPrimaryGhost>
                        <ThePlus />
                    </smPrimaryGhost>
                </div>
                <div class="blok-button">
                    <smSecondaryGhost>Button</smSecondaryGhost>
                    <smSecondaryGhost>
                        <ThePlus /> Button&ensp;
                    </smSecondaryGhost>
                    <smSecondaryGhost>&ensp;Button
                        <TheIconChevron />
                    </smSecondaryGhost>
                    <smSecondaryGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smSecondaryGhost>
                    <smSecondaryGhost>
                        <ThePlus />
                    </smSecondaryGhost>
                </div>
                <div class="blok-button">
                    <smDangerGhost>Button</smDangerGhost>
                    <smDangerGhost>
                        <ThePlus /> Button&ensp;
                    </smDangerGhost>
                    <smDangerGhost>&ensp;Button
                        <TheIconChevron />
                    </smDangerGhost>
                    <smDangerGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </smDangerGhost>
                    <smDangerGhost>
                        <ThePlus />
                    </smDangerGhost>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <mdPrimaryGhost>Button</mdPrimaryGhost>
                    <mdPrimaryGhost>
                        <ThePlus /> Button&ensp;
                    </mdPrimaryGhost>
                    <mdPrimaryGhost>&ensp;Button
                        <TheIconChevron />
                    </mdPrimaryGhost>
                    <mdPrimaryGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdPrimaryGhost>
                    <mdPrimaryGhost>
                        <ThePlus />
                    </mdPrimaryGhost>
                </div>
                <div class="blok-button">
                    <mdSecondaryGhost>Button</mdSecondaryGhost>
                    <mdSecondaryGhost>
                        <ThePlus /> Button&ensp;
                    </mdSecondaryGhost>
                    <mdSecondaryGhost>&ensp;Button
                        <TheIconChevron />
                    </mdSecondaryGhost>
                    <mdSecondaryGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdSecondaryGhost>
                    <mdSecondaryGhost>
                        <ThePlus />
                    </mdSecondaryGhost>
                </div>
                <div class="blok-button">
                    <mdDangerGhost>Button</mdDangerGhost>
                    <mdDangerGhost>
                        <ThePlus /> Button&ensp;
                    </mdDangerGhost>
                    <mdDangerGhost>&ensp;Button
                        <TheIconChevron />
                    </mdDangerGhost>
                    <mdDangerGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </mdDangerGhost>
                    <mdDangerGhost>
                        <ThePlus />
                    </mdDangerGhost>
                </div>
            </div>
            <div class="one-blok-button">
                <div class="blok-button">
                    <lgPrimaryGhost>Button</lgPrimaryGhost>
                    <lgPrimaryGhost>
                        <ThePlus /> Button&ensp;
                    </lgPrimaryGhost>
                    <lgPrimaryGhost>&ensp;Button
                        <TheIconChevron />
                    </lgPrimaryGhost>
                    <lgPrimaryGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgPrimaryGhost>
                    <lgPrimaryGhost>
                        <ThePlus />
                    </lgPrimaryGhost>
                </div>
                <div class="blok-button">
                    <lgSecondaryGhost>Button</lgSecondaryGhost>
                    <lgSecondaryGhost>
                        <ThePlus /> Button&ensp;
                    </lgSecondaryGhost>
                    <lgSecondaryGhost>&ensp;Button
                        <TheIconChevron />
                    </lgSecondaryGhost>
                    <lgSecondaryGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgSecondaryGhost>
                    <lgSecondaryGhost>
                        <ThePlus />
                    </lgSecondaryGhost>
                </div>
                <div class="blok-button">
                    <lgDangerGhost>Button</lgDangerGhost>
                    <lgDangerGhost>
                        <ThePlus /> Button&ensp;
                    </lgDangerGhost>
                    <lgDangerGhost>&ensp;Button
                        <TheIconChevron />
                    </lgDangerGhost>
                    <lgDangerGhost>
                        <ThePlus /> Button
                        <TheIconChevron />
                    </lgDangerGhost>
                    <lgDangerGhost>
                        <ThePlus />
                    </lgDangerGhost>
                </div>
            </div>

        </div>
    </div>
</template>

