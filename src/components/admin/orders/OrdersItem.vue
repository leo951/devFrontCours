<template>
    <div>
        <div class="order__card" v-if="ordersObject">
            <router-link :to="{name:'OrdersModify', params:{id:ordersObject._id}}">
                <h2>
                    Numéro de la commande: {{ordersObject._id}}
                </h2>
            </router-link>
            <h3>Date de la commande: {{ordersObject.date}}</h3>
            <h4>La commande est : {{ordersObject.status}}</h4>
               
        </div>
    </div>
</template>

<script>

    export default {
        name:"OrdersItem",
        created() {
        },
        props:{
            ordersObject: Object,
        },
       
        methods:{
        }
    }
</script>

<style lang="scss" scoped>

</style>