<script setup>
import {RouterLink} from 'vue-router'
import HomeIconVue from './icons/HomeIcon.vue';
import AboutIcon from './icons/AboutIcon.vue';
import ProjectsIcon from './icons/ProjectsIcon.vue';
import GithubIcon from './icons/GithubIcon.vue';
import LinkedinIcon from './icons/LinkedinIcon.vue';
</script>

<template>
    <header>
        <nav>
            <RouterLink to="/"><HomeIconVue class="icon"/></RouterLink>
            <RouterLink to="/about"><AboutIcon class="icon"/></RouterLink>
            <RouterLink to="/works"><ProjectsIcon class="icon"/></RouterLink>
        </nav>
    </header>
</template>

<style>
    header {
        position: absolute;
        left: 40px;
        top: 0;
        height: 100%;
    }

    header nav {
        display: flex;
        flex-flow: column nowrap;
        gap: 40px;
        justify-content: center;
        height: inherit;
    }

    header nav a {
        display: flex;
        flex-flow: row nowrap;
        align-items: center;
        gap: 10px;
        color: white;
        font-size: 18px;
        font-weight: 400;
        width: 200px;
        text-decoration: none;
    }

    .icon {
        width: 30px;
    }
    header nav a:hover{
        color: rgb(255, 206, 47);
    }
</style>