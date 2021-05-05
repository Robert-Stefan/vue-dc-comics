<template>
    <div class="box"> 
        <img :src="details.thumb" alt="" />
    </div>
</template>

<script>
export default {
    name: 'ProdCard',
    props: ['details'],
}
</script>

<style>

</style>