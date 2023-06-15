<template>
    <main>
        <h1>
             - - Content goes in here - - -
        </h1>
    </main>
</template>
<script>
export default {
    name: 'AppMain',
    data(){
        return{

        }
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

    }
</style>