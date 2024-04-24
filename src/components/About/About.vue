<template>
    <section class="uk-container uk-margin-large-top uk-margin-large-bottom" >
        <div class="uk-child-width-1-2@s uk-child-width-1-1" uk-grid uk-height-match="target: > div > .uk-card">
            <div class="uk-card ">
                <img :src="aboutImg" class="uk-img-mobile">
            </div>
            <div class="uk-card uk-margin-medium-top">
                <h1 class="uk-text-title">
                    Sobre a Two brothers Tech
                </h1>
                <h3 class="uk-margin-top uk-text-subTitle ">
                    Uma empresa nascida da paixão de dois irmãos pela tecnologia. Inicialmente fundada
                    por eles, cresceu ao atrair profissionais destacados do mercado de TI. Nosso time diversificado oferece
                    serviços especializados para impulsionar o crescimento dos clientes.<br>
                    Na Two Brothers Tech, unimos
                    expertise, criatividade e dedicação para criar sistemas robustos e personalizados, adaptados às
                    necessidades específicas de cada cliente.
                </h3>
                <div class="uk-text-center " style="margin-top: 55px;">
                    <button class="uk-margin-left button-prim">Quero conhecer</button>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'AboutApp',
    data() {
        return {
            aboutImg: require('./aboutImg.svg'),
        };
    },
};
</script>
<style scoped>
.uk-text-title {
    color: #191A15;
    font-size: 40px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    font-family: 'Inter', sans-serif;
    width: 420px;
}

.uk-text-subTitle {
    color: var(--Texto, #4F5052);
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 30px;
}

.button-prim {
    font-family: 'Inter', sans-serif;
    width: 261px;
    height: 45px;
    border-radius: 5px;
    background-color: #1E2643;
    border: none;
    color: var(--Branco, #FFF);
    font-size: 16px;
}
@media only screen and (max-width: 800px) {
.uk-img-mobile{
    margin-left: 25px;
}
.uk-text-title{
    font-size: 35px;
    width: 250px;
}
.uk-text-subTitle {
    font-size: 15px;
    width: 380px;
}
}
</style>
    