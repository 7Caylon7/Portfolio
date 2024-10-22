<template>
    <main class="parallax">
        <h2>Projects</h2>
    </main>
</template>

<script>
export default {
    name: 'ProjectsComponent'
}
</script>


<style scoped>
.parallax{
    background-image: url(../assets/bg-blue.jpg);
    min-height: 100%;
    height: 100vh;
    position: relative;
    opacity: 0.65;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
</style>