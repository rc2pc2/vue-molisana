<template>
    <div>
        <h1>
            La mia prima app con Vite!
        </h1>
        <img src="../assets/vue.svg" alt="Vue Logo">
    </div>
</template>

<script>
export default {
    name: 'MainNavbar',
    data(){
        return{

        }
    },

    methods: {
        getImagePath: function(img) {
            return new URL(`../assets/${img}`, import.meta.url).href;
        }
    }
}
</script>

<style lang="">

</style>