<script setup>
import GithubIcon from './icons/GithubIcon.vue';
import LinkedinIcon from './icons/LinkedinIcon.vue';
</script>

<template>
    <footer>
        <nav>
            <a href="https://github.com/santanderson"><GithubIcon class="icon"/></a>
            <a href="https://www.linkedin.com/in/anderson-ryan-fernandes-924a0422a/"><LinkedinIcon class="icon"/></a>
        </nav>
    </footer>
</template>

<style>
    footer{
        position: absolute;
        right: 80px;
        bottom: 40px;
    }
    footer nav {
        display: flex;
        flex-flow: row nowrap;
        gap: 30px;
    }
    footer nav a {
        color: white;
    }
    footer nav a:hover .icon{
        color: rgb(255, 206, 47);
    }
</style>