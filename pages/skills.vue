<template id="skills">
    <section class="skills section">
        <h2 class="section__title">Skills</h2>
        <span class="section__subtitle">My favorite skills</span>

        <div class="skills__container container grid section__border">
            
            <div class="skills__content">
                <h3 class="skills__title">
                    <i class="ri-braces-line"></i> FullStack Web/Mobile Developer
                </h3>

                <div class="skills__info" >
                    <div class="skills__data" v-for="skill in skills" :key="skill.name">
                        <div class="skills__blob">
                            <img :src="skill.img" :alt="skill.name">
                        </div>

                        <h3 class="skills__name">{{ skill.name }}</h3>
                        <span class="skills__subtitle">{{ skill.level }}</span>
                    </div>

                    <!-- <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/css-3.svg" alt="">
                        </div>

                        <h3 class="skills__name">CSS</h3>
                        <span class="skills__subtitle">Advance</span>
                    </div>

                    <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/logo-javascript.svg" alt="">
                        </div>

                        <h3 class="skills__name">JAVASCRIPT</h3>
                        <span class="skills__subtitle">Advanced</span>
                    </div>

                    <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/react-2.svg" alt="">
                        </div>

                        <h3 class="skills__name">REACT</h3>
                        <span class="skills__subtitle">Intermediate</span>
                    </div>

                    <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/git-icon.svg" alt="">
                        </div>

                        <h3 class="skills__name">GIT</h3>
                        <span class="skills__subtitle">Intermediate</span>
                    </div>

                    <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/figma-1.svg" alt="">
                        </div>

                        <h3 class="skills__name">TYPESCRIPT</h3>
                        <span class="skills__subtitle">Intermediate</span>
                    </div>

                    <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/figma-1.svg" alt="">
                        </div>

                        <h3 class="skills__name">NODE</h3>
                        <span class="skills__subtitle">Intermediate</span>
                    </div>
                    
                    <div class="skills__data">
                        <div class="skills__blob">
                            <img src="../assets/img/figma-1.svg" alt="">
                        </div>

                        <h3 class="skills__name">POSTGRESS</h3>
                        <span class="skills__subtitle">Intermediate</span>
                    </div> -->

                </div>

            </div>

        </div>
    </section>
</template>

<script setup>
import typescriptLogo from "~/assets/img/typescript-2.svg"
import figmaLogo from "~/assets/img/go-6.svg"

    const skills = ref([
        {name: 'TypeScript', img: typescriptLogo , level: 'Intermediate'},
        {name: 'Go', img: typescriptLogo, level: 'Intermediate'},
        {name: 'Vue', img: figmaLogo, level: 'Intermediate'},
        {name: 'Nuxt', img: figmaLogo, level: 'Intermediate'},
        {name: 'Next', img: figmaLogo, level: 'Intermediate'},
        {name: 'Nest', img: figmaLogo, level: 'Intermediate'},
        {name: 'Prisma', img: figmaLogo, level: 'Intermediate'},
        {name: 'Tailwindcss', img: figmaLogo, level: 'Intermediate'},
        {name: 'Git', img: figmaLogo, level: 'Intermediate'},
    ])
</script>

<style scoped>

</style>