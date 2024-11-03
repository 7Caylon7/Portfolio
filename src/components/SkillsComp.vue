<template>
    <div class="background">
        <h3 class="d-flex justify-content-center" style="font-family: 'Courier New', Courier, monospace;font-weight: 600;">Hard Skills</h3>
        <div class="skills">
            <div class="skills-slide">
                <i style="color: #bf2626;" class="mdi mdi-language-html5"></i>
                <i style="color: #288ba8;" class="mdi mdi-language-css3"></i>
                <i style="color: #f2b138;" class="mdi mdi-language-javascript"></i>
                <i style="color: #746ab0;" class="mdi mdi-language-php"></i>
                <i class="mdi mdi-language-python python-icon"></i>
                <i style="color: #00ffab;" class="mdi mdi-vuejs"></i>
                <i style="color: #746ab0;" class="mdi mdi-bootstrap"></i>
                <i style="color: #00ffab;" class="mdi mdi-bulma"></i>
                <i style="color: #161310;" class="mdi mdi-github"></i>
                <i style="color: #fc3f00;" class="mdi mdi-gitlab"></i>
                <i style="color: #d02090;" class="mdi mdi-database"></i>
                <i style="color: #d06060;" class="mdi mdi-api"></i>
            </div>
            <div class="skills-slide">
                <i style="color: #bf2626;" class="mdi mdi-language-html5"></i>
                <i style="color: #288ba8;" class="mdi mdi-language-css3"></i>
                <i style="color: #f2b138;" class="mdi mdi-language-javascript"></i>
                <i style="color: #746ab0;" class="mdi mdi-language-php"></i>
                <i class="mdi mdi-language-python python-icon"></i>
                <i style="color: #00ffab;" class="mdi mdi-vuejs"></i>
                <i style="color: #746ab0;" class="mdi mdi-bootstrap"></i>
                <i style="color: #00ffab;" class="mdi mdi-bulma"></i>
                <i style="color: #161310;" class="mdi mdi-github"></i>
                <i style="color: #fc3f00;" class="mdi mdi-gitlab"></i>
                <i style="color: #d02090;" class="mdi mdi-database"></i>
                <i style="color: #d06060;" class="mdi mdi-api"></i>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SkillsComponent'
}
</script>


<style scoped>
.background{
    background-color: #ECEBEB;
}

i{
    font-size: 400%;
    margin: 0 5vw;
}

.python-icon{
    background: linear-gradient(135deg, #306998 40%, #FFD43B 60%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.skills{
    overflow: hidden;
    white-space: nowrap;
}

.skills-slide{
    display: inline-block;
    animation: 15s slide infinite linear;
}

@keyframes slide {
    from{
        transform: translateX(0);
    }
    to{
        transform: translateX(-100%);
    }
    
}
</style>