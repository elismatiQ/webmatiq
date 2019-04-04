<template>
    <div class="util__flex" v-editable="blok">
        <component :key="blok.uid" v-for="blok in blok.columns" :blok="blok" :is="blok.component"></component> 
    </div>
</template>

<script>
export default {
    props: ['blok']
}
</script>