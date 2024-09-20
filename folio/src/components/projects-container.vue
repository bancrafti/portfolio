<template>
    <div class="project-container">
        <div class="project-image"><img src="" alt=""></div>
    </div>
</template>
<style scoped>
.project-container {
    position: fixed;
    width: 90%;
    max-width: 30%;
    top: 150px;
    bottom: 10%;
    left: 75.1%;
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
    .project-container {
        width: 80%;
        top: 5%;
        bottom: 5%;
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