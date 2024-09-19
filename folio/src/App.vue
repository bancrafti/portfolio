<script>
import PhotoContainer from './components/photo-container.vue';
import HeaderContainer from './components/header-container.vue';
import WorkContainer from './components/work-container.vue';
import ProjectsContainer from './components/projects-container.vue';

export default {
    components: {
        HeaderContainer,
        PhotoContainer,
        WorkContainer,
        ProjectsContainer
    }
}
</script>

<template>

    <body>
        <HeaderContainer />
        <WorkContainer />
        <PhotoContainer />
        <ProjectsContainer />
    </body>

</template>
<style scoped>
body {
    padding: 100px;
}
</style>