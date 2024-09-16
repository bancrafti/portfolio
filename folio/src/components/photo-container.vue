<template>
    <div class="photo-container">
        <img src="" alt="Photograph" class="profile-photo">
    </div>
</template>
<style scoped>
.photo-container {
    position: fixed;
    width: 20%;
    height: 600px;
    top: 150px;
    left: 32%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: inherit;
    border-radius: inherit;
    padding: auto;
    box-sizing: border-box;
    flex-shrink: 0;
}

.profile-photo {
    border-radius: 50%;
    width: 100px;
    height: 100px;
    object-fit: cover;
}
</style>