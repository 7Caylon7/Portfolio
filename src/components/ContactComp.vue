<template>
  <div class="parallax" id="contact">
    <div class="container">
      <div class="main d-flex flex-direction-row">
        <form class="form" action="https://formsubmit.co/caylonsolon@hotmail.com" method="POST">

          <button class="btn-contato">
            <span> Contact me </span>
          </button>

          <input class="form-control" type="text" placeholder="Nome" required />
          <input class="form-control" type="email" name="email" placeholder="E-mail" required />
          <textarea class="form-control" rows="6" name="description" id="description"
            placeholder="Descreva o seu projeto ou problema!!" required></textarea>
          <button class="btn-enviar" type="submit">
            <span class="icon mdi mdi-email email"></span>
            <p class="text">Enviar</p>
          </button>

          <input type="hidden" name="_next" value="https://portfolio-solon.vercel.app">

          <input type="hidden" name="_captcha" value="false" />
          <input type="hidden" name="_subject" value="Novo Contato!" />
          <input type="text" name="_honey" style="display: none" />
        </form>
        <div class="links">
          <div class="up">
            <a class="card1" href="https://www.instragram.com/ca_ylon/profilecard/?igsh=YnptaGp3MXFhZmdj"
              target="_blank">
              <i class="instagram mdi mdi-instagram"></i>
            </a>
            <a class="card2" href="https://www.linkedin.com/in/caylon-solon-monte-costa" target="_blank">
              <i class="twitter mdi mdi-linkedin"></i>
            </a>
          </div>
          <div class="down">
            <a class="card3" href="https://github.com/7Caylon7" target="_blank"><i
                class="github mdi mdi-github "></i></a>
            <a class="card4" href="">
              <i class="discord mdi mdi-whatsapp "></i>
            </a>
          </div>
        </div>
      </div>
      <div>
        <footer class="d-flex flex-wrap justify-content-between align-items-center- py-3 my-4 border-top">
          <p class="col-md-4 mb-0">@ 2024 Caylon Solon</p>
          <h3 class="nav">
            <i class="mdi mdi-chevron-left"></i>Solon/<i class="mdi mdi-chevron-right"></i>
          </h3>
        </footer>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactComponent",
};
</script>

<style scoped>
.parallax {
  background-image: url(../assets/bg-gray.avif);
  position: relative;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}

.main {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  height: 87vh;
  font-family: "Roboto", sans-serif;
  color: #ecebee;
}

.btn-contato {
  padding: 0.1em 0.25em;
  width: 13em;
  height: 4.2em;
  background-color: #212121;
  border: 0.08em solid #fff;
  border-radius: 0.3em;
  font-size: 12px;
  cursor: pointer;
}

.btn-contato span {
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
  font-family: 'Courier New', Courier, monospace;
}

.btn-contato span:hover {
  transition: all 0.5s;
  transform: translate(0, 0.4em);
  box-shadow: 0 0 0 0 #fff;
}

.btn-contato span:not(hover) {
  transition: all 1s;
}


.form {
  display: flex;
  flex-direction: column;
  align-items: center;
  flex-wrap: wrap;
  width: 35vw;
  height: 50vh;
  gap: 2vh;
}

.btn-enviar {
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

.icon {
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

.text {
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

.btn-enviar:hover .icon {
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

footer {
  color: #ecebee;
}

footer>h3 {
  font-family: "Courier New", Courier, monospace;
}

footer>p {
  font-family: "Roboto", sans-serif;
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
  box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px,
    rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  transition: 0.2s ease-in-out;
}

.instagram {
  position: relative;
  left: 1.5vw;
  top: 1.5vh;
  color: #cc39a4;
  font-size: 300%;
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
  box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px,
    rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  transition: 0.2s ease-in-out;
}

.twitter {
  position: relative;
  left: 0.7vw;
  top: 1.5vh;
  color: #03a9f4;
  font-size: 300%;
}

.card3 {
  width: 90px;
  height: 90px;
  outline: none;
  border: none;
  background: white;
  border-radius: 5px 5px 5px 90px;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px,
    rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  transition: 0.2s ease-in-out;
}

.github {
  position: relative;
  left: 1.5vw;
  top: .6vh;
  font-size: 300%;
  color: #000;
}

.card4 {
  width: 90px;
  height: 90px;
  outline: none;
  border: none;
  background: white;
  border-radius: 5px 5px 90px 5px;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px,
    rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  transition: 0.2s ease-in-out;
}

.discord {
  position: relative;
  left: .7vw;
  top: .6vh;
  color: #6dfabf;
  font-size: 300%;
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
  background-color: #03a9f4;
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

@media (max-width: 599px) {
  .main {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .form {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 65vw;
    height: 50vh;
    gap: 2vh;
  }

  h3 {
    font-size: large;
  }

  textarea {
    height: 6vh;
  }

  .btn-enviar {
    width: 100%;
  }

  .icon {
    width: 10vw;
  }

  .text {
    margin-top: 2.2vh;
  }

  .instagram {
    left: 7vw;
    top: 1.5vh;
  }

  .twitter {
    left: 4vw;
    top: 1.5vh;
  }

  .github {
    left: 7vw;
    top: .6vh;
  }

  .discord {
    left: 4vw;
    top: .6vh;
  }

}


@media (min-width: 600px) and (max-width: 899px) {
  h3 {
    font-size: large;
  }

  textarea {
    height: 17vh;
  }

  .btn-enviar {
    width: 100%;
  }

  .icon {
    width: 10vw;
  }

  .text {
    margin-top: 2.2vh;
  }

  .instagram {
    left: 4vw;
    top: 1.5vh;
  }

  .twitter {
    left: 1.2vw;
    top: 1.5vh;
  }

  .github {
    left: 4vw;
    top: .6vh;
  }

  .discord {
    left: 1.2vw;
    top: .6vh;
  }
}


@media (min-width: 900px) and (max-width: 1199px) {

  textarea {
    height: 10vh;
  }

  .btn-enviar {
    width: 100%;
  }

  .icon {
    width: 10vw;
  }

  .text {
    margin-top: 1vh;
  }

  .instagram {
    left: 3vw;
    top: 1.5vh;
  }

  .twitter {
    left: 1.2vw;
    top: 1.5vh;
  }

  .github {
    left: 3vw;
    top: .6vh;
  }

  .discord {
    left: 1.2vw;
    top: .6vh;
  }

  footer {
    margin: 0;
    padding: 0;
  }
}

@media (min-width: 1200px) and (max-width: 1599px) {
  .form {
    height: 60vh;
    gap: 2vh;
  }

  .instagram {
    left: 2vw;
    top: 1.5vh;
  }

  .twitter {
    left: 1.2vw;
    top: 1.5vh;
  }

  .github {
    left: 2vw;
    top: .6vh;
  }

  .discord {
    left: 1.2vw;
    top: .6vh;
  }
}
</style>
