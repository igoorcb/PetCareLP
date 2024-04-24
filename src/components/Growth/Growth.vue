<template >
    <div style="background-color: #EFEFEF;">
        <section class="uk-container">
            <div class="uk-child-width-1-2@s uk-child-width-1-1 uk-margin-large-top" uk-grid uk-height-match="target: > div > .uk-card">
                <figure>
                    <h1 class="uk-text-title">
                        Impulsionando o seu crescimento
                    </h1>
                    <h3 class="uk-margin-top uk-text-subTitle">
                        Já imaginou ter tudo isso e muito mais para o seu negócio
                    </h3>
                    <div v-for="(icons, index) in icons" :key="index"  class="uk-margin-top">
                        <img :src="icons.src">
                        <span class="uk-margin-left uk-text-one">{{ icons.text }}</span>
                        <div class="uk-margin-subText uk-text-two">
                            <span>{{ icons.subText }}</span>
                        </div>
                    </div> 
                </figure>
                <div class="uk-margin-large-top">
                    <img :src="Growth">
                </div>
            </div>
        </section>
    </div>
</template>
<script>
export default {
    name: 'GrowthApp',
    data() {
        return {
            Growth: require('./Growth.svg'),
            icons: [
                { src: require('./icon_one.svg'), text: 'Ganho em produtividade', subText: 'Mapeamos o seu negócio e desenvolvemos uma solução de ponta a ponta, reduzindo em até 50% o seu tempo em processos morosos' },
                { src: require('./icon_two.svg'), text: 'Experiência do Usuário Incrível', subText: 'Priorizamos interfaces fáceis de usar e atraentes. Com nosso design amigável, sua equipe e clientes terão uma experiência positiva ao interagir com os sistemas, aumentando a produtividade e satisfação.' },
                { src: require('./icon_three.svg'), text: 'Soluções Integradas e Eficientes', subText: 'A adoção de práticas de desenvolvimento ágil permite entregas contínuas e iterativas, garantindo que as soluções atendam rapidamente às necessidades do cliente.' },
            ],
        };
    },
};
</script>
<style scoped>
.uk-text-title {
    color: #191A15;
    font-family: 'Inter', sans-serif;
    font-size: 40px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}
.uk-text-one{
    color: var(--Texto, #4F5052);
    font-family: 'Inter', sans-serif;
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
.uk-text-two{
    color: var(--Texto, #4F5052);
    font-family: 'Inter', sans-serif;
    font-size: 15px;
    font-style: normal;
    font-weight: 400;
    line-height: 25px; 
}
.uk-text-subTitle {
    color: rgba(79, 80, 82, 0.80);
    font-family: 'Inter', sans-serif;
    font-size: 17px;
    font-style: normal;
    font-weight: 400;
    line-height: 30px;
}
.uk-margin-subText{
    margin-left: 60px;
}
@media only screen and (max-width: 800px) {
.uk-text-title {
    font-size: 35px;
    width: 300px ;
}
.uk-text-subTitle{
    font-size: 15px;
}
.uk-text-one{
    font-size: 18px;
}
.uk-text-two{
font-size: 15px;
}
}
</style>
    