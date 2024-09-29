<template>
    <div class="header-container">
        <h1>WARIBU</h1>
        <div class="menu-icon" @click="toggleMenu">
            &#9776;
        </div>
        <nav :class="['nav-links', { 'nav-active': isMenuActive }]">
            <a href="#projects">PROJECTS</a>
            <a href="#about">ABOUT</a>
            <a href="#contact">CONTACT</a>
        </nav>
    </div>
    <div class="work-container">
        <p class="job-description">Passionate and detail-oriented <a class="slim">frontend developer</a> </p>
    </div>
    <div class="photo-container">
        <img src="/home/waribu/workspace/portfolio/folio/src/assets/me.jpeg" alt="Photograph" class="profile-photo">
    </div>
    <div class="project-container">
        <div class="project-image"><img src="" alt=""></div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isMenuActive: false
        };
    },
    methods: {
        toggleMenu() {
            this.isMenuActive = !this.isMenuActive;
        }
    }
};
</script>

<style scoped>
.header-container {
    position: relative;
    border-radius: var(--Rounded, 20px);
    background: var(--Primary, #000000);
    display: flex;
    width: 90vw;
    max-width: 100vw;
    height: 80px;
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

.menu-icon {
    display: none;
    font-size: 2rem;
    cursor: pointer;
    color: pink;
    position: absolute;
    right: 20px;
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

.nav-links a:hover {
    color: white; 
    font-weight: bolder;
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

    .menu-icon {
        display: block;
    }

    .nav-links {
        display: none;
        flex-direction: column;
        width: 100%;
        justify-content: space-around;
        margin-top: 10px;
    }

    .nav-links.nav-active {
        display: flex;
    }
}

.work-container {
    position: fixed;
    width: 33vw;
    height: 50vh;
    top: 120px;
    left: 5vw;
    right: 34px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: var(--Primary, #000000);
    border-radius: var(--Rounded, 20px);
    padding: 10px;
    box-sizing: border-box;
    flex-shrink: 0;
}

.job-description {
    font-size: 40px;
    color: white;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    padding: 20px;
}

.slim {
    font-weight: 100;
    color: pink;
}

.photo-container {
    position: fixed;
    width: 20dvw;
    height: 50dvh;
    top: 120px;
    left: 39dvw;
    display: flex;
    justify-content: center;
    align-items: center;
    background: var(--Primary, #000000);
    border-radius: var(--Rounded, 20px);
    padding: auto;
    box-sizing: border-box;
    flex-shrink: 0;
}

.profile-photo {
    border-radius: var(--Rounded, 20px);
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.project-container {
    position: fixed;
    width: 35vw;
    max-width: 90vw;
    top: 120px;
    height: 65vh;
    left: 77.5vw;
    transform: translateX(-50%);
    display: flex;
    justify-content: center;
    align-items: center;
    background: var(--Primary, #000000);
    border-radius: var(--Rounded, 20px);
    padding: 10px;
    box-sizing: border-box;
    flex-shrink: 0;
}

@media (max-width: 768px) {
    .work-container,
    .photo-container,
    .project-container {
        position: static;
        width: 90%;
        height: auto;
        margin: 10px auto;
    }

    .job-description {
        font-size: 1.5rem;
        text-align: center;
    }

    .profile-photo {
        width: 100%;
        height: auto;
    }
}

@media (max-width: 480px) {
    .project-container {
        width: 95%;
        top: 2%;
        bottom: 2%;
    }
}
</style>