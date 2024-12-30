<template>
    <div class="photo-container">
        <img src="/home/waribu/workspace/portfolio/folio/src/assets/me.jpeg" alt="Photograph" class="profile-photo">
    </div>
</template>
<style scoped>
.photo-container {
    position: fixed;
    width: 20%;
    height: 600px;
    top: 150px;
    left: 39%;
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
</style>