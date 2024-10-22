<template>
    <div class="about-container">
        <section ref="textSection">
            <p v-show="!showSecondParagraph" class="firstParagraph">
                Olá, eu sou Caylon Solon, desenvolvedor web Jr com mais de três anos de experiência na área. Atualmente,
                estou cursando o oitavo semestre de Engenharia da Computação, uma jornada que me permite aprofundar
                ainda mais minha paixão por tecnologia e resolução de problemas. Desde cedo, fui fascinado pelo poder
                transformador da tecnologia, e isso me levou a me especializar em desenvolvimento web, onde vejo a
                oportunidade de facilitar e otimizar tarefas diárias através de soluções criativas e funcionais.
            </p>
            <p v-show="showSecondParagraph" class="secondParagraph">
                Hoje, atuo como desenvolvedor na ASTTIC-UFPA em regime de estágio, onde aplico meus conhecimentos na
                criação e manutenção de sistemas que impactam diretamente a rotina de diversas pessoas. Meu maior sonho
                é, no futuro, liderar uma equipe de desenvolvedores, seja como gerente de projetos ou em outro cargo de
                liderança, contribuindo com inovação e inspirando outros a seguirem o mesmo caminho de transformação
                tecnológica.
            </p>
        </section>
        <aside ref="imageAside">
            <img src="../assets/ilustracao.webp" alt="Ilustração de desenvolvedor">
        </aside>
    </div>
</template>

<script>
import gsap from "gsap";

export default {
    name: 'AboutComponent',
    data() {
        return {
            showSecondParagraph: false // Estado para controlar qual parágrafo mostrar
        };
    },

    mounted() {
        // Animações de entrada
        gsap.from(this.$refs.textSection, {
            x: '-100%',  // O parágrafo vem da esquerda
            opacity: 0,  
            duration: 1.5, 
            ease: 'power2.out', 
        });

        gsap.from(this.$refs.imageAside, {
            x: '100%',  // A imagem vem da direita 
            opacity: 0,
            duration: 1.5,
            ease: 'power2.out',
        });

        // Adiciona um listener para o evento de scroll
        window.addEventListener('scroll', this.handleScroll);
    },

    beforeUnmount() {
        // Remove o listener ao destruir o componente
        window.removeEventListener('scroll', this.handleScroll);
    },

    methods: {
        handleScroll() {
            const scrollPosition = window.scrollY;
            const triggerPosition = 0.1;

            // Se a posição do scroll for maior que a posição de acionamento, mostra o segundo parágrafo
            if (scrollPosition > triggerPosition && !this.showSecondParagraph) {
                this.showSecondParagraph = true; // Mostra o segundo parágrafo
                gsap.fromTo(this.$refs.textSection.querySelector('.secondParagraph'), {
                    opacity: 0,
                    y: 20
                }, {
                    opacity: 1, // Fica visível
                    y: 0, // Move para a posição original
                    duration: 0.5,
                    ease: 'power2.out'
                });
            } else if (scrollPosition <= triggerPosition && this.showSecondParagraph) {
                this.showSecondParagraph = false; // Mostra o primeiro parágrafo
                gsap.fromTo(this.$refs.textSection.querySelector('.firstParagraph'), {
                    opacity: 0, 
                    y: 20 // Move para baixo
                }, {
                    opacity: 1,
                    y: 0, // Move para a posição original
                    duration: 0.5,
                    ease: 'power2.out'
                });
            }
        }
    }
}
</script>

<style scoped>
.about-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    background-color: #ECEBEB;
    padding: 10%;
    height: 100vh;
}

section {
    flex: 1;
    position: relative;
}

aside {
    flex: 1;
    display: flex;
    justify-content: center;
}

section p {
    font-weight: 400;
    font-size: medium;
    line-height: 1.8;
    font-family: 'Roboto', sans-serif;
    transition: opacity 0.5s ease; /* Transição suave ao mudar a opacidade */
}

aside img {
    width: 100%;
    max-width: 100vh;
    height: auto;
    margin-left: 25%;
    border-radius: 50%;
}
</style>
