<template>
    <nav>
        <h3 class="d-flex justify-content-center" style="font-family: 'Playfair Display', sans-serif;font-weight: 400;">Skills</h3>
        <ul class="d-flex flex-row justify-content-xl-around">
            <li style="color: #bf2626;"><i class="mdi mdi-language-html5"></i></li>
            <li style="color: #288ba8;"><i class="mdi mdi-language-css3"></i></li>
            <li style="color: #f2b138;"><i class="mdi mdi-language-javascript"></i></li>
            <li style="color: #746ab0;"><i class="mdi mdi-language-php"></i></li>
            <li class="python-icon"><i class="mdi mdi-language-python"></i></li>
            <li style="color: #00ffab;"><i class="mdi mdi-vuejs"></i></li>
            <li style="color: #746ab0;"><i class="mdi mdi-bootstrap"></i></li>
            <li style="color: #00ffab;"><i class="mdi mdi-bulma"></i></li>
            <li style="color: #161310;"><i class="mdi mdi-github"></i></li>
            <li style="color: #fc3f00;"><i class="mdi mdi-gitlab"></i></li>
            <li style="color: #d02090;"><i class="mdi mdi-database"></i></li>
            <li style="color: #d06060;"><i class="mdi mdi-api"></i></li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'SkillsComponent'
}
</script>


<style scoped>
nav{
    background-color: #ECEBEB;   
}

li{
    font-size: 350%;
}

ul{
    margin-bottom: 0;
}

.python-icon{
    background: linear-gradient(135deg, #306998 40%, #FFD43B 60%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

</style>