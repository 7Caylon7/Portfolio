<template>
    <main class="parallax">
        <div class="container">
            <button>
                <span> Projects </span>
            </button>
        </div>
        <div class="container">
            <ul class="d-flex flex-row justify-content-around">
                <li class="card" style="width: 25vw; background-color: #ECEBEB;">
                    <img class="rounded" src="../assets/pj-filmes.png" alt="imagem de um site de filmes">
                    <ul class="d-flex flex-row justify-content-around" style="padding: 0; height: 5vh;">
                        <li style="color: #00ffab; font-size: 200%;"><i class="mdi mdi-vuejs"></i></li>
                        <li style="color: #746ab0; font-size: 200%;"><i class="mdi mdi-bootstrap"></i></li>
                        <li style="color: #288ba8; font-size: 200%;"><i class="mdi mdi-language-css3"></i></li>
                        <li style="color: #f2b138; font-size: 200%;"><i class="mdi mdi-language-javascript"></i></li>
                        <li style="color: #d06060; font-size: 200%;"><i class="mdi mdi-api"></i></li>
                        <li style="font-size: 200%;">
                            <a class="btn-go" href="https://movies-solon.vercel.app" target="_blank">
                                <i class="mdi mdi-arrow-top-right-bold-box-outline"></i>
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="card" style="width: 25vw; background-color: #ECEBEB;">
                    <img class="rounded" src="../assets/pj-pkdx.png" alt="imagem de um site de filmes">
                    <ul class="d-flex flex-row justify-content-around" style="padding: 0; height: 5vh;">
                        <li style="color: #00ffab; font-size: 200%;"><i class="mdi mdi-vuejs"></i></li>
                        <li style="color: #288ba8; font-size: 200%;"><i class="mdi mdi-language-css3"></i></li>
                        <li style="color: #006494; font-size: 200%;"><i class="mdi mdi-language-typescript"></i></li>
                        <li style="color: #d06060; font-size: 200%;"><i class="mdi mdi-api"></i></li>
                        <li style="font-size: 200%;">
                            <a class="btn-go" href="https://pokedex-7ca.vercel.app" target="_blank">
                                <i class="mdi mdi-arrow-top-right-bold-box-outline"></i>
                            </a>
                        </li>
                    </ul>
                </li>
            </ul>
            <ul class="d-flex flex-row justify-content-around">
                <li class="card" style="width: 25vw; background-color: #ECEBEB;">
                    <img class="rounded" src="../assets/pj-barber.png" alt="imagem de um site de filmes">
                    <ul class="d-flex flex-row justify-content-around" style="padding: 0; height: 5vh;">
                        <li style="color: #00ffab; font-size: 200%;"><i class="mdi mdi-vuejs"></i></li>
                        <li style="color: #288ba8; font-size: 200%;"><i class="mdi mdi-language-css3"></i></li>
                        <li style="font-size: 200%;">
                            <a class="btn-go" href="https://jp-barbearia.vercel.app" target="_blank">
                                <i class="mdi mdi-arrow-top-right-bold-box-outline"></i>
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="card" style="width: 25vw; background-color: #ECEBEB;">
                    <img class="rounded" src="../assets/pj-api.png" alt="imagem de um site de filmes">
                    <ul class="d-flex flex-row justify-content-around" style="padding: 0; height: 5vh;">
                        <li style="color: #f2b138; font-size: 200%;"><i class="mdi mdi-language-javascript"></i></li>
                        <li style="color: #d06060; font-size: 200%;"><i class="mdi mdi-api"></i></li>
                        <li style="font-size: 200%;">
                            <a class="btn-go" href="https://filmes-api-sandy.vercel.app" target="_blank">
                                <i class="mdi mdi-arrow-top-right-bold-box-outline"></i>
                            </a>
                        </li>
                    </ul>
                </li>
            </ul>
        </div>
    </main>
</template>

<script>
export default {
    name: 'ProjectsComponent'
}
</script>


<style scoped>
.parallax {
    background-image: url(../assets/bg-blue.jpg);
    height: 100vh;
    position: relative;
    opacity: 0.65;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.container {
    padding-top: 2%;
}

.btn-go{
    color: #161310;
    transition: transform 0.3s ease;
}

.btn-go:hover{
    transform: scale(1.5);
}

button {
    padding: 0.1em 0.25em;
    width: 13em;
    height: 4.2em;
    background-color: #212121;
    border: 0.08em solid #fff;
    border-radius: 0.3em;
    font-size: 12px;
    cursor: pointer;
}

button span {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    bottom: 0.4em;
    width: 8.25em;
    height: 2.5em;
    background-color: #212121;
    border-radius: 0.2em;
    font-size: 1.5em;
    color: #fff;
    border: 0.08em solid #fff;
    box-shadow: 0 0.4em 0.1em 0.019em #fff;
}

button span:hover {
    transition: all 0.5s;
    transform: translate(0, 0.4em);
    box-shadow: 0 0 0 0 #fff;
}

button span:not(hover) {
    transition: all 1s;
}
</style>