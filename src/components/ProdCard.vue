<template>
    <div class="box"> 
        <img :src="details.thumb" :alt="details.type" />
        <p> {{ details.series }}</p>
    </div>
</template>

<script>
export default {
    name: 'ProdCard',
    props: ['details'],

    // posso fare anche
    // props: { details: String o Array o Object },
}
</script>

<style scoped lang="scss">
    .box {
        flex-basis: calc((100% / 6) - 10px);
        color: white;
        p {
            padding: 20px 0;
        }

        img {
            cursor: pointer;
        }
    }
</style>