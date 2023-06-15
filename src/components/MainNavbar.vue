<template>
    <div>
        <div class="container">
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur provident, explicabo modi facere quibusdam enim eaque tempore odio vitae deleniti ut totam iure minus quasi necessitatibus suscipit sed aliquam! Nobis!</p>

            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur provident, explicabo modi facere quibusdam enim eaque tempore odio vitae deleniti ut totam iure minus quasi necessitatibus suscipit sed aliquam! Nobis!</p>

            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur provident, explicabo modi facere quibusdam enim eaque tempore odio vitae deleniti ut totam iure minus quasi necessitatibus suscipit sed aliquam! Nobis!</p>
        </div>
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

<style lang="scss">
    $primary_color : #fff;

    @mixin flex($direction: row, $justify: center, $align: center , $wrap: wrap){
        display: flex;
        flex-direction: $direction;
        justify-content: $justify;
        align-items: $align;
        flex-wrap: $wrap;
    }

    div.container{
        @include flex(column, center, start, nowrap);
        background-color: $primary_color;
    }
</style>