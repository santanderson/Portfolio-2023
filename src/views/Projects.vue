<script setup>
const projects = [
    {
        name: 'Google Interface',
        img: './src/assets/images/google-interface.png',
        link: 'https://santanderson.github.io/Google-Interface/',
        desc: 'Cópia da ui do google.com'
    },
    {
        name: 'Google Interface',
        img: './src/assets/images/google-interface.png',
        link: 'https://santanderson.github.io/Google-Interface/',
        desc: 'Cópia da ui do google.com'
    },
    {
        name: 'Google Interface',
        img: './src/assets/images/google-interface.png',
        link: 'https://santanderson.github.io/Google-Interface/',
        desc: 'Cópia da ui do google.com'
    },
    {
        name: 'Google Interface',
        img: './src/assets/images/google-interface.png',
        link: 'https://santanderson.github.io/Google-Interface/',
        desc: 'Cópia da ui do google.com'
    },
    {
        name: 'Google Interface',
        img: './src/assets/images/google-interface.png',
        link: 'https://santanderson.github.io/Google-Interface/',
        desc: 'Cópia da ui do google.com'
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
                        <div class="info">
                            <h3>{{ project.name }}</h3>
                            <span>{{project.desc}}</span>
                        </div>
                        <img :src="project.img" :alt="project.name"/>
                    </a>
                </div>

            </div>
        </section>
    </main>
</template>