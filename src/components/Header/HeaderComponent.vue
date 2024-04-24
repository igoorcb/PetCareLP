<template>
  <header class="uk-height-img uk-flex-middle uk-background-cover uk-light" :data-src="backgroundImageUrl" uk-img>
    <div class="uk-container uk-container-large ">
      <section class="uk-position-relative">
        <div class="uk-margin-medium-top">
          <img :src="LogoImageUrl">
        </div>
        <ul class="uk-position-bottom-right uk-padding-small">
          <a href="#Serviços" uk-scroll>
            <span class="uk-nav-text uk-nav-text-mb uk-margin-left">Serviços</span>
          </a>
          <a href="#Sobre" uk-scroll>
            <span class="uk-nav-text uk-nav-text-mb uk-margin-left">Sobre nós</span>
          </a>
          <a href="#Clientes" uk-scroll>
            <span class="uk-nav-text uk-nav-text-mb uk-margin-left">Clientes</span>
          </a>
        </ul>
      </section>
      <section>
        <div class="uk-margin-section">
          <h1 class="uk-text-one ">Desenvolvemos a solução ideal para o seu negócio!</h1>
          <h1 class="uk-text-two">Potencialize seu sucesso e eficiência com nossos sistemas personalizados. Soluções
            incríveis para impulsionar o crescimento do seu negócio de forma eficaz e inovadora.</h1>
        </div>
        <div class="uk-margin-large-top">
          <a href="https://api.whatsapp.com/send?phone=5531993928387" target="_blank">
            <button class="uk-button-wpp">
              <span class="uk-text-button">Solicitar contato no WhatsApp</span>
              <img :src="IconWpp" class="uk-margin-left">
            </button>
          </a>
        </div>
      </section>
    </div>
  </header>
</template>
<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      backgroundImageUrl: require('./background.png'),
      LogoImageUrl: require('./Logo2BT.png'),
      IconWpp: require('./iconWpp.svg'),
    };
  },
};
</script>
<style scoped>
.uk-height-img {
  height: 950px;
}

.uk-nav-text {
  color: var(--Branco, #FFF);
  font-family: 'Inter', sans-serif;
  font-size: 18px;
  font-style: normal;
  font-weight: 500;
  line-height: normal;
}

.uk-text-one {
  color: var(--Branco, #FFF);
  font-family: 'Inter', sans-serif;
  font-size: 55px;
  font-style: normal;
  font-weight: 700;
  line-height: 80px;
  width: 700px;
}

.uk-text-two {
  color: var(--Branco, #FFF);
  font-family: 'Inter', sans-serif;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: 25px;
  width: 670px;
}

.uk-margin-section {
  margin-top: 170px;
}

.uk-button-wpp {
  width: 356px;
  height: 50px;
  flex-shrink: 0;
  border-radius: 5px;
  background: #12D1B6;
  box-shadow: 0px 8px 24px 0px rgba(0, 0, 0, 0.15);
  border-color: #12D1B6;
}

.uk-text-button {
  color: var(--Preto, #1E2643);
  font-family: 'Inter', sans-serif;
  text-align: center;
  font-size: 14px;
  font-style: normal;
  font-weight: 600;
  line-height: 30px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

@media only screen and (max-width: 800px) {
  .uk-nav-text-mb {
    font-size: 14px;
  }

  .uk-text-one {
    font-size: 35px;
    width: 320px;
    line-height: 50px;
  }

  .uk-text-two {
    font-size: 20px;
    line-height: 25px;
    width: 350px;
  }
}</style>
