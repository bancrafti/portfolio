<template>
    <div class="main-container">
        <div class="work-container">
            <p class="job-description">
                Code whisperer turning <span class="highlight">caffeine</span> and curiosity into clever solutions
            </p>
        </div>

        <div class="photo-container">
        </div>

        <div class="project-container">
            <h2>Tech Stack</h2>
            <div class="stack-section">
                <p>Technical languages</p>
                <div class="tech-icons">
                    <img v-for="tech in techLanguages" :key="tech.name" :src="tech.icon" :alt="tech.name">
                </div>
                <p>Frameworks & Technologies</p>
                <div class="tech-icons">
                    <img v-for="framework in frameworks" :key="framework.name" :src="framework.icon"
                        :alt="framework.name">
                </div>
            </div>
        </div>

        <div class="description-container">
            <p class="description-text">
                Waribu is a passionate software engineer with a knack for crafting innovative solutions, leveraging
                technology
                to solve complex problems, and delivering impactful user experiences
            </p>
        </div>

        <div class="contact-container">
            <div class="contact-text">Contact me</div>
            <div class="contact-arrow">↗</div>
        </div>

        <div class="links-container">
            <div class="navigation-links">
                <a v-for="link in links" :key="link" href="#">{{ link }}</a>
            </div>
        </div>
    </div>
</template>

<script setup>
const techLanguages = [
    { name: 'Python', icon: 'python-icon.png' },
    { name: 'HTML', icon: 'html-icon.png' },
    { name: 'JavaScript', icon: 'js-icon.png' },
    { name: 'SQL', icon: 'sql-icon.png' },
    { name: 'Flutter', icon: 'flutter-icon.png' },
    { name: 'Git', icon: 'git-icon.png' },
    { name: 'CSS', icon: 'css-icon.png' },
    { name: 'C++', icon: 'c-icon.png' }
];

const frameworks = [
    { name: 'React', icon: 'react-icon.png' },
    { name: 'Django', icon: 'django-icon.png' },
    { name: 'Vue', icon: 'vue-icon.png' },
    { name: 'Next.js', icon: 'next-icon.png' }
];

const links = ['EMAIL', 'GITHUB', 'LINKEDIN'];
</script>

<style src="./assets/main.css"></style>
