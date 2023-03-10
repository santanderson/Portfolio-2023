<script setup>
import data from "../assets/data.json";

console.log(data.projects)

const projects = data.projects

</script>

<template>
    <main>
        <section>
            <h2>Projetos</h2>

            <div class="projectsContainer">

                <div v-for="project in projects">
                    <a :href="project.url" target="_blank">
                        <div class="info">
                            <h3>{{ project.name }}</h3>
                            <span>{{project.description}}</span>
                        </div>
                        <img :src="project.imgPath" :alt="project.name"/>
                    </a>
                </div>

            </div>
        </section>
    </main>
</template>