<template>
    <div class="header-container">
        <h1>WARIBU</h1>
        <nav class="nav-links">
            <a href="#projects">PROJECTS</a>
            <a href="#about">ABOUT</a>
            <a href="#contact">CONTACT</a>
        </nav>
    </div>
    <div class="work-container">
    </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.header-container {
    border-radius: var(--Rounded, 20px);
    background: var(--Primary, #000000);
    display: flex;
    width: calc(100% - 40px);
    max-width: calc(100% - 400px);
    height: 101px;
    padding: 10px 50px 0px 50px;
    justify-content: space-between;
    align-items: center;
    flex-shrink: 0;
    position: fixed;
    top: 24px;
    left: 50%;
    transform: translateX(-50%);
    z-index: 1000;
    box-sizing: border-box;
}

.header-container h1 {
    font-family: 'Sans', serif;
    font-size: 2rem;
    font-weight: bold;
    color: pink;
}

.nav-links {
    display: flex;
    gap: 20px;
}

.nav-links a {
    text-decoration: none;
    color: pink;
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
        left: 50%;
        transform: translateX(-50%);
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