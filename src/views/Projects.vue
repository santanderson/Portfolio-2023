<script setup>
const projects = [
    {
        name: 'BluOcean',
        img: 'src',
        link: 'google.com'
    }
]
</script>

<template>
    <main>
        <section>
            <h2>Projetos</h2>

            <div class="projectsContainer">
                <div v-for="project in projects">
                    <a :href="project.link" target="_blank">
                        <h3>{{ project.name }}</h3>
                        <img src="" :alt="project.name"/>
                    </a>
                </div>
            </div>
        </section>
    </main>
</template>