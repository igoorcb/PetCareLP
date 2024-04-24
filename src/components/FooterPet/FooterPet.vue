<template >
    <div class="uk-background-color-footer">
        <section class="uk-container ">
            <div class="uk-child-width-1-2 uk-child-width-1-2 uk-margin-large-top" uk-grid>
                <!-- <div>
                    <h1 class="uk-text-title">Temos a melhor solução para você</h1>
                    <h1 class="uk-text-subTitle">Digite seu WhatsApp e um dos nossos especialistas entrará em contato</h1>
                </div> -->
                <!-- <div class="uk-margin-medium-top">
                    <div class="uk-margin-large-left">
                        <span class="uk-text-input">Vamos conversar?</span>
                    </div>
                    <div class="uk-margin-large-left">
                        <input-footer >
                            <input class="uk-input uk-margin-small-top size-button" type="text" placeholder="(DDD) + número" aria-label="Input">
                        </input-footer>
                        <img :src="Send" alt="" class="send-button">
                    </div>
                </div> -->
            </div>
            <div class="uk-text-center uk-margin-large-top">
                <img :src="LogoImageUrl">
            </div>
            <div class="uk-text-center uk-margin-large-top uk-margin-large-bottom uk-text-footer">
                2BT © 2023 Todos os Direitos Reservados
            </div>
        </section>
    </div>
</template>
<script>
export default {
    name: 'FooterPet',
    data() {
    return {
      LogoImageUrl: require('./Logo2BT.png'),
      Send: require('./Send.svg'),
    };
  },
};
</script>
<style scoped>
.uk-background-color-footer {
    background: var(--Preto, #1E2643);
}
.size-button{
    width: 400px;
    height: 45px;
    justify-content: center;
    align-items: center;
    flex-shrink: 0;
    background: #FFF;
}
.send-button{
    width: 59px;
    height: 45px;
    flex-shrink: 0;
    margin-top: 10px;
}
.uk-text-footer{
    color: var(--Branco, #FFF);
    text-align: center;
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 30px; 
    }
.uk-text-title{
    color: #FFF;
    font-family: 'Inter', sans-serif;
    font-size: 40px;
    font-style: normal;
    font-weight: 600;
    line-height: normal; 
}
.uk-text-subTitle{
    color: #E6E9F5;
    font-family: 'Inter', sans-serif;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.uk-text-input{
    color: #FEFEFE;
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 30px; 
}
@media only screen and (max-width: 800px) {
 
}
</style>
    