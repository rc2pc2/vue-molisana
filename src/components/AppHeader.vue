<template>
    <header>
        <div id="brand">
            <img src="../assets/img/la-molisana-logo.png" alt="La Molisana main logo">
        </div>
        <nav id="top-navbar">
            <ul>
                <li>
                    Home
                </li>
                <li class="active">
                    Prodotti
                </li>
                <li>
                    Chi siamo
                </li>
                <li>
                    Contatti
                </li>
            </ul>
        </nav>
    </header>
</template>
<script>
export default {
    name: 'AppHeader',
    data(){
        return{

        }
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    header{
        display: flex;
        flex-direction: column;

        div#brand img{
            height: 110px;
            display: block;
            margin: 0 auto;
            margin-bottom: 2rem;
        }

        nav#top-navbar ul{
            @include flex();
            margin-bottom: 2rem;

            li{
                padding: 1rem;
                font-size: .9rem;
                font-weight: 600;
                // background: $acc;
                transition: background-color 1s ease;

                &.active,
                &:hover{
                    background-color: $accentBg;
                }
            }
        }
    }

</style>