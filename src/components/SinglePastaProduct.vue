<template lang="">
    <article>
        <h3>
            {{ pastaElement.titolo }}
        </h3>
        <div class="picture">
            <img :src="pastaElement.src" alt="">
        </div>
        <p class="cooking-time">
            {{ pastaElement.cottura }}
        </p>
    </article>
</template>
<script>
export default {
    name: 'SinglePastaProduct',
    props: {
        pastaElement : Object
    },
    // props: [
    //     'pastaElement'
    // ]
}
</script>
<style lang="scss" scoped>
    article{
        width: calc((100% / 4) - 3px);
        background-color: white;
        padding: 1rem;
        margin-right: 3px;
        margin-bottom: 3px;

        img{
            width: 100%;
        }
    }
</style>