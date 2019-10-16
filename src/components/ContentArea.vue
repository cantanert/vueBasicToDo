<template>
    <div class="contentArea container">
        <AddItem></AddItem>
        <ListingItem></ListingItem>
    </div>
</template>

<script>


    import AddItem from "./AddItem";
    import ListingItem from "./ListingItem";

    export default {
        name: "ContentArea",
        components: {
            AddItem,
            ListingItem
        }
    }
</script>

<style scoped>
    .contentArea{
        width: 50%;
        margin-top: 100px;
        margin-bottom: 100px;
    }
</style>