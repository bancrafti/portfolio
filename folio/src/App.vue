<script>
import PhotoContainer from './components/photo-container.vue';
import HeaderContainer from './components/header-container.vue';
import WorkContainer from './components/work-container.vue';

export default {
    components: {
        HeaderContainer,
        PhotoContainer,
        WorkContainer,
    }
}
</script>

<template>
    <HeaderContainer />
    <WorkContainer/> 
    <PhotoContainer/>
</template>