<template>
    <main>
        <h1>
            Lista Prodotti:
        </h1>
        <PastaProducts class="container"/>
    </main>
</template>
<script>
import PastaProducts from './PastaProducts.vue';

export default {
    name: 'AppMain',
    data(){
        return{

        }
    },
    components:{
        PastaProducts
    }
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    main{
        background-image: url('../assets/img/fondo-pag-speciali.jpg');
        color: $primaryColor;
        padding: 3rem;
        text-align: center;
        font-size: .75rem;
        margin-bottom: $sectionsMargin;

        h1{
            margin-bottom: $sectionsMargin;
        }
    }
</style>