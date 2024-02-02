<script>
export default {
    name: 'ComicsCard',
    props: {
        currentSeries: Object

    },
}
</script>



<template>
    <div class="cards-col">
        <div class="comic-card">
            <figure>
                <img :src="currentSeries.thumb" :alt="currentSeries.series">
            </figure>
            <h4>{{ currentSeries.series }}</h4>
        </div>
    </div>
</template>
<style scoped lang="scss">
img {
    max-height: 169px;
}
</style>