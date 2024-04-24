<template >
    <div id="Clientes"/>
    <section class="uk-container uk-margin-large-top" >
        <div class="uk-text-center">
            <h1 class="uk-text-title">Clientes especiais</h1>
            <h1 class="uk-text-subTitle ">O que nossos clientes<br> estão dizendo</h1>
        </div>
        <div class="uk-grid-small uk-child-width-1-2@s uk-margin-top uk-margin-large-bottom "  uk-grid>
            <div v-for="(icon, index) in icons" :key="index">
                <div class="uk-card uk-card-default uk-card-body uk-margin-medium-top uk-card-border ">
                    <img class="uk-margin-img" :src="icon.src" alt="Icon Image">
                    <div class="uk-img-size">
                        <img :src="aspas">
                    </div>
                    <div class="uk-text-abt uk-margin-left">
                        {{ icon.text }}
                    </div>
                    <div class="uk-text-name uk-margin-medium-top uk-margin-left">
                        {{ icon.name }}
                    </div>
                    <div class="uk-text-companyName uk-margin-left ">
                        {{ icon.companyName }}
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'GrowthApp',
    data() {
        return {
            aspas: require('./aspas.svg'),
            icons: [
                { src: require('./icon_one.svg'), text: 'Gostamos muito do trabalho, equipe bem profissional, conhecimento vasto de programação agregando muito valos aos projetos desempenhados.', name: 'Matheus Franquini', companyName: 'Empresas&Negócios' },
                { src: require('./icon_two.svg'), text: 'Excelente experiência com a 2BT. Desenvolveram um app com profissionalismo e eficiência. Comunicação clara, prazos cumpridos e qualidade excepcional. Recomendo!', name: 'Ana Paula Paiva', companyName: 'PetCare' },
            ],
        };
    },
};
</script>
<style scoped>
.uk-img-size {
    width: 15px;
    margin-top: 20px;
}

.uk-text-abt {
    color: var(--Texto, #4F5052);
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 30px; 
}

.uk-text-name {
    color: var(--Neutral-900, #111827);
    font-family: 'Inter', sans-serif;
    font-feature-settings: 'liga' off;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: 28px;
    }

.uk-text-companyName {
    color: var(--Label, #8D8D8D);
    font-family: 'Inter', sans-serif;
    font-size: 13px;
    font-style: normal;
    font-weight: 400;
    line-height: 30px; 
}

.uk-margin-img {
    margin-left: -7px;
}

.uk-text-title {
    color: #09AD96;
    font-family: 'Inter', sans-serif;
    text-align: center;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
}

.uk-text-subTitle {
    color: #191A15;
    font-family: 'Inter', sans-serif;
    text-align: center;
    font-size: 40px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin-top: -10px;
}
.uk-card-border{
    border-radius: 15px;
    border: 1px solid #F7F7F7;
    background: var(--Branco, #FFF);
    box-shadow: 3px 4px 17px 0px rgba(159, 159, 159, 0.25);
    flex-shrink: 0;
}
@media only screen and (max-width: 800px) {
 .uk-text-title{
    font-size: 13px;
 }
 .uk-text-subTitle{
    font-size: 25px;
 }   
}
</style>
    