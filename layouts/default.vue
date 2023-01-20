<template>
    <div>
        <header>
            <nav>
                <a href="#">Toby</a>

                <ul>
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="skills">Skills</NuxtLink></li>
                    <li><NuxtLink to="qualifications">Qualifications</NuxtLink></li>
                    <li><NuxtLink to="projects">Projects</NuxtLink></li>
                </ul>
            </nav>
        </header>

        <slot />
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>