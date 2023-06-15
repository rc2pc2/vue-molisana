<template>
    <footer>
        <div class="footer-brand">
            <img src="../assets/img/la-molisana-logo.png" alt="Stylized mountains background">
        </div>
        <nav class="pastas-footer">
            <h2>
                Pastificio
            </h2>
            <ul>
                <li><a href="#">Il Pastificio</a></li>
                <li><a href="#">Grano</a></li>
                <li><a href="#">Filiera</a></li>
                <li><a href="#">100 anni di pasta</a></li>
                <li><a href="#">Sartoria della pasta</a></li>
            </ul>
        </nav>
        <nav class="products-footer">
            <h2>
                Prodotti
            </h2>
            <ul>
                <li><a href="#">Le classiche</a></li>
                <li><a href="#">Le Integrali</a></li>
                <li><a href="#">Le Speciali</a></li>
                <li><a href="#">Le Biologiche</a></li>
                <li><a href="#">Le Gluten-free</a></li>
            </ul>
        </nav>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter',
    data(){
        return{

        }
    }
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    footer{
        @include flex();
        background-image: url('../assets/img/footer-montagne-bottom.jpg');
        background-repeat: no-repeat;
        background-position: bottom;
        background-size: contain;
        padding-bottom: calc($sectionsMargin * 6);

        &>*{
            margin-right: 6rem;
        }

        h2{
            font-size: 1.15rem;
            text-transform: uppercase;
            color: $primaryColor;
            font-weight: 600;
            margin-bottom: .85rem;
        }

        div.footer-brand img{
            height: 80%;
            display: block;
            margin: 0 auto;
        }

    }

</style>