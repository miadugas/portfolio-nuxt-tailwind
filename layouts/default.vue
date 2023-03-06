<template>
    <div>
        <header>
            <nav>
                    <li><NuxtLink to="/">Mia Codes</NuxtLink></li>
                <ul>
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/splash">A Tech Splash</NuxtLink></li>
                    <li><NuxtLink to="/portfolio">Portfolio</NuxtLink></li>
                    <li><NuxtLink to="/about">About Me</NuxtLink></li>
                    <li><NuxtLink to="/estimate">Estimate</NuxtLink></li>
                    <li><NuxtLink to="/contact">Contact Me</NuxtLink></li>
                </ul>
            </nav>
        </header>
<!-- page content -->
<div>
    <slot />
</div>
    </div>
</template>

<style scoped>
    .router-link-exact-active {
    color: #12b488;
    }
</style>