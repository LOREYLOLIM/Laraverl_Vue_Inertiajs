<script setup>
import Projects from "@/Components/Frontend/Projects.vue";
import Project from "@/Components/Frontend/Project.vue";
import {p} from "../../../../public/build/assets/app-709e09a6.js";

defineProps({
    skills:Object,
    projects: Object,
})
</script>

<template>
    <section id="portfolio" class="section bg-light-primary dark:bg-dark-navy-primary min-h-[1400]">
        <div class="container mx-auto">
            <div class="flex flex-col items-center text-center">
                <h2 class="section-title">My Latest Work</h2>
                <p class="subtitle">
                    Loremdssjbsj sbsfjsbjsf jbjbgafa jadggajjabdja dajdjabjad mdbshdjs
                </p>
            </div>
        </div>
        <Projects :skills="skills" :projects="projects"/>
    </section>
    <section class="grid gap-y-12 lg:grid-cols-3 lg:gap-8">
        <Project v-for="project in projects" :key="project.id" :project="project"/>
    </section>
</template>

<style scoped>

</style>
