<template>
    <div class="category__card" v-if="categoryObject">
        <router-link :to="{name:'CategoryAdmin', params:{id:categoryObject._id}}">
            <h2>
                {{categoryObject.title}}
            </h2>
        </router-link>
    </div>
</template>

<script>
    export default {
        name:"CategoryItem",
        created() {
            },
        props:{
            categoryObject: Object,
        }
    }
</script>

<style lang="scss" scoped>

</style>
