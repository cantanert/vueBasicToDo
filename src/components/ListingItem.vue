<template>
    <div class="listingItem">
        <p class=" itemText animated bounce" v-for="item in data" :class="{'animated bounce' : removing}"  :key="item">{{item}} <i class="fa fa-minus-circle" @click="removeEmit(item)"></i></p>
    </div>
</template>

<script>
    export default {
        name: "ListingItem",
        props: ['data','removing'],
        methods:{
            removeEmit(param){
                this.$emit("remove-item",param);
            }
        }
    }
</script>

<style scoped>
    .listingItem{
        width: 100%;
    }
    .itemText{
        padding: 0 10px;
        background-color: gainsboro;
        margin: 2px 0;
        text-align: left;
    }
    .itemText i{
        float: right;
        cursor: pointer;
        line-height: 1.3;
    }
</style>