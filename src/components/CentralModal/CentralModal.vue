<template >
  <div id="Serviços">
  <section class="uk-container uk-container-medium uk-margin-bkc uk-visible@m" >
    <div class="uk-child-width-1-3 uk-grid-small uk-margin-left " uk-grid>
      <div v-for="(icons, index) in icons" :key="index" >
        <div class="uk-card uk-card-body ">
          <img :src="icons.src" class="uk-text-start">
          <div >
            <h1 class="uk-text-pr uk-margin-top">{{ icons.text }}</h1>
          </div>
          <div class="uk-margin-top">
            <h1 class="uk-text-sub">{{ icons.subText }}</h1>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section class="uk-container uk-container-small uk-margin-bkc uk-hidden@l uk-size-mobile" >
    <div class="uk-child-width-1-2 uk-grid-small " uk-grid>
      <div v-for="(icons, index) in icons" :key="index">
        <div class="uk-card uk-card-body uk-margin-bottom-mb">
          <img :src="icons.src" class="uk-text-start">
          <div>
            <h1 class="uk-text-pr uk-margin-top">{{ icons.text }}</h1>
          </div>
          <div class="uk-margin-top">
            <h1 class="uk-text-sub">{{ icons.subText }}</h1>
          </div>
        </div>
      </div>
    </div>
  </section>
</div > 
<div id="Sobre" />
</template>
<script>
export default {
  name: 'CentralModal',
  data() {
    return {
      icons: [
        { src: require('./icons/icon_one.svg'), text: 'Desenvolvimento ágil', subText: 'Uma abordagem flexível para entrega rápida e eficiente de sistemas' },
        { src: require('./icons/icon_two.svg'), text: 'Migração de banco de dados', subText: 'Transferência segura e eficiente de dados entre sistemas' },
        { src: require('./icons/icon_three.svg'), text: 'API’s e Integrações', subText: 'Conectividade perfeita para potencializar a sua rotina' },
        { src: require('./icons/icon_four.svg'), text: 'UX/UI Design', subText: 'Aprimore a experiência do usuário com interfaces intuitivas e agradaveis' },
        { src: require('./icons/icon_five.svg'), text: 'Infraestrutura e nuvem', subText: 'Tenha uma base sólida para sistemas inovadores, escaláveis e seguros' },
        { src: require('./icons/icon_six.svg'), text: 'Mais vendas e segurança', subText: 'Potencialize seu negócio online com confiança e eficiência.' },
      ],
    };
  },
};
</script>
<style scoped>
.uk-margin-bkc {
  margin-top: -150px;
  border-radius: 10px;
  border: 1px solid #EFEFEF;
  background: var(--Branco, #FFF);
  box-shadow: 9px 12px 40px 0px rgba(186, 186, 186, 0.25);
}
.uk-text-pr{
  color: var(--Titulo, #242423);
  font-family: 'Inter', sans-serif;
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
}
.uk-text-sub{
  color: var(--Label, #8D8D8D);
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 20px;
  width: 218px;
}
.uk-size-text{
  width: 220px;
}
@media only screen and (max-width: 800px) {
.uk-text-pr{
  font-size: 14px;
  line-height: normal;
  width: 140px;
}
.uk-text-sub{
  font-size: 12px;
  line-height: 20px;
  width: 140px;
}
.uk-size-mobile{
  width: 360px;
  height: 625px;
}
.uk-margin-bkc {
  margin-top: -170px;
}
.uk-margin-bottom-mb{
  margin-bottom: -60px;
  padding-top: 20px;
}
}

</style>
  