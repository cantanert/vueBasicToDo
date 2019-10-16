<template>
    <div class="listingItem">
        <p v-for="item in items" :key="item">{{item}}</p>
    </div>
</template>

<script>
    export default {
        name: "ListingItem",
        data(){
            return {
                items: {
                    0 : "Sıfır",
                    1 : "Bir"
                }
            }
        }
    }
</script>

<style scoped>
    /*.listingItem{
        width: 100%;
    }*/
</style>