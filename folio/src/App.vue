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
    <div class="photo-container"><img src="" alt="" class="profile-photo"> </div>
    </div>
</template>
<style scoped>
.header-container {
    border-radius: var(--Rounded, 20px);
    background: var(--Primary, #646464);
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
    font-family: 'Sans', serif;
    font-size: 2rem;
    font-weight: bold;
    color: var(--Text, #ffffff);
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

.work-container {
    position: fixed;
    width: 30%;
    height: 600px;
    top: 150px;
    left: 24px;
    right: 24px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: var(--Primary, #646464);
    border-radius: var(--Rounded, 20px);
    padding: 10px;
    box-sizing: border-box;
    flex-shrink: 0;
}
.photo-container{
    position: fixed;
    width: 20%;
    height: 600px;
    top: 150px;
    left: 32%;
    display:flex;
    justify-content: center;
    align-items: center;
    background: inherit;
    border-radius: inherit;
    padding: auto;
    box-sizing: border-box;
    flex-shrink: 0;
}
.profile-photo{
    border-radius: 50%;
    width: 100px;
    height: 100px;
    object-fit: cover;
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

    .photo-container {
        top: 130px;
        /* Adjust this value as needed for smaller screens */
        left: 10px;
        right: 10px;
    }

    .profile-photo {
        width: 80px;
        height: 80px;
    }
}
</style>