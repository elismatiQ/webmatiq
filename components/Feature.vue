<template>
    <div class="feature util__flex-eq" v-editable="blok">
        <img :src="resizedIcon" class="feature__icon">
        <h2>{{ blok.name }}</h2>
        <div class="feature__description">
            {{ blok.description }}
        </div>
    </div>
</template>

<script>
export default {
    computed: {
        resizedIcon () {
            if (typeof this.blok.icon !== 'undefined') {
                return '//img2.storyblok.com/80x80' + this.blok.icon.replace('//a.storyblok.com', '')
            }
            return null
        }
    },
    props: ['blok']
}
</script>

<style lang="scss">
.feature {
    text-align: center;
    padding: 30px 10px 100px;
}

.feature__icon {
    max-width: 80px;
}
</style>
