<template>
    <div>
        <header class="header">
            <nav class="nav container">
                <a href="#" class="nav__logo">Toby</a>

                <div class="nav__menu" :class="{show: menu}">
                    <ul class="nav__list grid">
                        <li class="nav__item" @click="showMenu">
                            <NuxtLink to="/" class="nav__link">
                                <i class="ri-home-5-line"></i>
                                Home
                            </NuxtLink>
                        </li>

                        <li class="nav__item" @click="showMenu">
                            <NuxtLink to="skills" class="nav__link">
                                <i class="ri-trophy-line"></i>
                                Skills
                            </NuxtLink>
                        </li>

                        <li class="nav__item" @click="showMenu">
                            <NuxtLink to="qualifications" class="nav__link">
                                <i class="ri-book-open-line"></i>
                                Qualifications
                            </NuxtLink>
                        </li>

                        <li class="nav__item" @click="showMenu">
                            <NuxtLink to="projects" class="nav__link">
                                <i class="ri-image-line"></i>
                                Projects
                            </NuxtLink>
                        </li>
                    
                    </ul>

                    <!-- Close button -->
                    <div class="nav__close" @click="showMenu">
                     <i class="ri-close-line"></i>
                    </div>
                </div>

                <div class="nav__buttons">
                    <!-- Theme change button -->
                    <div class="change-theme" @click="toggleDark()">
                        <i v-if="isDark" class="ri-moon-line" ></i>
                        <i v-else class="ri-sun-line"></i>
                    </div>
                    <div class="nav__toggle" @click="showMenu">
                        <i class="ri-menu-4-line"></i>
                    </div>
                </div>
                
            </nav>
        </header>

        <slot />
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    import {useDark, useToggle} from '@vueuse/core'
    import 'remixicon/fonts/remixicon.css'

    
    const isDark = useDark();
    const toggleDark = useToggle(isDark);

    const menu = ref(false);

    const showMenu = () =>  menu.value = !menu.value;
    
</script>

<style >
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&family=Roboto:wght@400;500&display=swap");

/*=============== VARIABLES CSS ===============*/

</style>