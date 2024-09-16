<template>
    <div class="header-container">
        <h1>Waribu</h1>
        <nav class="nav-links">
            <a href="#projects">PROJECTS</a>
            <a href="#about">ABOUT</a>
            <a href="#contact">CONTACT</a>
        </nav>
    </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.header-container {
    border-radius: var(--Rounded, 20px);
    background: var(--Primary, #000000);
    display: flex;
    width: calc(100% - 24px);
    max-width: calc(100% - 40px);
    height: 101px;
    padding: 10px 25px 0px 24px;
    justify-content: space-between;
    align-items: center;
    flex-shrink: 0;
    position: fixed;
    top: 24px;
    left: 24px;
    right: 20px;
    z-index: 1000;
    box-sizing: border-box;
    padding: 20px;
}

.header-container h1 {
    font-family: 'monospace';
    font-size: 2rem;
    font-weight: bold;
    color: var(--Text, #fdfdfd);
}

.nav-links {
    display: flex;
    gap: 20px;
}

.nav-links a {
    text-decoration: none;
    color: var(--Text, #ffffff);
    font-family: 'Arial', sans-serif;
    font-size: 1.25rem;
    font-weight: 500;
    text-transform: uppercase;
}

@media (max-width: 768px) {
    .header-container {
        height: auto;
        padding: 10px;
        width: calc(100% - 20px);
        max-width: calc(100% - 20px);
        left: 10px;
        right: 10px;
        flex-direction: column;
        align-items: flex-start;
    }

    .header-container h1 {
        font-size: 1.5rem;
    }

    .nav-links {
        width: 100%;
        justify-content: space-around;
        margin-top: 10px;
    }
}
</style>