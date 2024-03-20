
<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <header>
        <nav class="container">
            <div class="branding">
                <h1>TODO</h1>
                <h2>LIST</h2>
            </div>
            <ul class="nav-routes">
                <RouterLink to="/">Home</RouterLink>
                <RouterLink to="/about">About</RouterLink>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    .branding {
        display: flex;
        align-items: center;
        h1 {
            font-size: x-large;
            font-weight: bolder;
            color: purple;
        }
        h2 {
            font-size: x-large;
            font-weight: 200;
            color: #1d1d1d;
        }
    }
}

nav ul {
    display: flex;
    gap: 12px;

    a {
    list-style: none;
    text-decoration: none;
    color: #1d1d1d;
    }
}
</style>