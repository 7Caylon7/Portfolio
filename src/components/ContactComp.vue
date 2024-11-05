<template>
    <div class="parallax" id="contact">
        <div class="container">
            <div class="main d-flex flex-direction-row">
                <form class="form" action="https://formsubmit.io/send/caylon.solon23@gmail.com" method="POST">
                    <h3>Me conte sobre o problema à ser resolvido!!</h3>
                    <input class="form-control" type="text" placeholder="Nome" required>
                    <input class="form-control" type="text" placeholder="E-mail" required>
                    <textarea class="form-control" rows="8" name="description" id="description" placeholder="Descreva o seu projeto" required></textarea>
                    <button class="btn-enviar" type="submit">
                        <span class="icon mdi mdi-email email"></span>
                        <p class="text">Enviar</p>
                    </button>

                    <input type="hidden" name="_captcha" value="false">
                    <input type="hidden" name="_subject" value="Novo Contato!">
                    <input type="text" name="_honey" style="display:none">
                </form>
                <div class="links">
                    <div class="up">
                        <button class="card1">
                            <a href="https://www.instragram.com/ca_ylon/profilecard/?igsh=YnptaGp3MXFhZmdj" target="_blank"><i class="mdi mdi-instagram instagram"></i></a>
                        </button>
                        <button class="card2">
                            <a href="https://www.linkedin.com/in/caylon-solon-monte-costa" target="_blank"><i class="mdi mdi-linkedin twitter"></i></a>
                        </button>
                    </div>
                    <div class="down">
                        <button class="card3">
                            <a href="https://github.com/7Caylon7" target="_blank"><i class="mdi mdi-github github"></i></a>
                        </button>
                        <button class="card4">
                            <i class="mdi mdi-whatsapp discord"></i>
                        </button>
                    </div>
                </div>
            </div>
            <div>
                <footer class="d-flex flex-wrap justify-content-between align-items-center- py-3 my-4 border-top">
                    <p class="col-md-4 mb-0">
                        @ 2024 Caylon Solon
                    </p>
                    <h3 class="nav"><i class="mdi mdi-chevron-left"></i>Solon/<i class="mdi mdi-chevron-right"></i></h3>
                </footer>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ContactComponent'
}
</script>

<style scoped>
.parallax {
    background-image: url(../assets/bg-blue.jpg);
    position: relative;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 100vh;
}


.main{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    height: 87vh;
}

.form{
    display: flex;
    flex-direction: column;
    align-items: center;
    flex-wrap: wrap;
    width: 35vw;
    height: 50vh;
    gap: 2vh;
}

.btn-enviar{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 20vw;
    height: 7vh;
    border-radius: 40px;
    border: 1px solid rgba(255, 255, 255, 0.349);
    background-color: rgb(12, 12, 12);
    cursor: pointer;
    transition-duration: 0.3s;
    overflow: hidden;
    color: #ecebee;
}

.icon{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 3vw;
    height: 6vh;
    background: linear-gradient(to bottom, rgb(83, 83, 83), rgb(43, 38, 48));
    border-radius: 50%;
    overflow: hidden;
    z-index: 2;
    transition-duration: 0.3s;
    font-size: 3vh;
}

.text{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    width: 60px;
    z-index: 1;
    transition-duration: 0.3s;
    font-size: 1.04em;
    margin-top: 1.2vh;
}

.btn-enviar:hover .icon{
    width: 100vw;
    height: 100vh;
    transition-duration: 0.3s;
}

.btn-enviar:hover .text {
  transform: translate(10px);
  width: 0;
  font-size: 0;
  transition-duration: 0.3s;
}

.btn-enviar:active {
  transform: scale(1.25);
  transition-duration: 0.3s;
}


footer{
    color: #ecebee;
}

.links {
    display: flex;
    flex-direction: column;
    gap: 0.5em;
}

.up {
    display: flex;
    flex-direction: row;
    gap: 0.5em;
}

.down {
    display: flex;
    flex-direction: row;
    gap: 0.5em;
}

.card1 {
    width: 90px;
    height: 90px;
    outline: none;
    border: none;
    background: white;
    border-radius: 90px 5px 5px 5px;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
    transition: .2s ease-in-out;
}

.instagram {
    margin-top: 1.5em;
    margin-left: .5em;
    color: #cc39a4;
    font-size: 200%;
}

.instagram:hover,
.twitter:hover,
.github:hover,
.discord:hover {
    color: #ecebee;
}

.card2 {
    width: 90px;
    height: 90px;
    outline: none;
    border: none;
    background: white;
    border-radius: 5px 90px 5px 5px;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
    transition: .2s ease-in-out;
}

.twitter {
    margin-top: 1.5em;
    margin-left: -.5em;
    color: #03A9F4;
    font-size: 200%;
}

.card3 {
    width: 90px;
    height: 90px;
    outline: none;
    border: none;
    background: white;
    border-radius: 5px 5px 5px 90px;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
    transition: .2s ease-in-out;
}

.github {
    margin-top: -.6em;
    margin-left: .5em;
    font-size: 200%;
    color: #000;
}

.card4 {
    width: 90px;
    height: 90px;
    outline: none;
    border: none;
    background: white;
    border-radius: 5px 5px 90px 5px;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
    transition: .2s ease-in-out;
}

.discord {
    margin-top: -.9em;
    margin-left: -.5em;
    color: #6dfabf;
    font-size: 200%;
}


.card1:hover {
    cursor: pointer;
    scale: 1.1;
    background-color: #cc39a4;
}

.card1:hover .instagram {
    fill: white;
}

.card2:hover {
    cursor: pointer;
    scale: 1.1;
    background-color: #03A9F4;
}

.card2:hover .twitter {
    fill: white;
}

.card3:hover {
    cursor: pointer;
    scale: 1.1;
    background-color: black;
}

.card3:hover .github {
    fill: white;
}

.card4:hover {
    cursor: pointer;
    scale: 1.1;
    background-color: #70ff8f;
}

.card4:hover .discord {
    fill: white;
}

</style>
