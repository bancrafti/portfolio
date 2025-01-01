<template>
    <div class="work-container">
        <p class="job-description">Passionate and detail-oriented <a class="slim">software developer</a> </p>
    </div>
    <div class="photo-container">
        <img src="/home/waribu/workspace/portfolio/folio/src/assets/me.jpeg" alt="Photograph" class="profile-photo">
    </div>
    <div class="project-container">
        <div class="project-image"><img src="" alt=""></div>
    </div>
    <div class="contact-container">
        <div class="contact-text">Contact me</div>
        <div class="contact-arrow">↗</div>
    </div>
    <div class="description-container">
        <div class="description-text"></div>
    </div>
    <div class="links-container">
        <div class="navigation-links">
            <a href="#">Email</a>
            <a href="#">Github</a>
            <a href="#">LinkedIn</a>
        </div>
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
