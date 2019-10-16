<template>
    <div class="contentArea container">
        <AddItem @add-item="addItem"></AddItem>
        <ListingItem @remove-item="removeItem" :data="items"></ListingItem>
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
        },
        data(){
            return {
                items: ["Bir","iki","üç","dört"]
            }
        },
        methods: {
            removeItem(param){
                var index = this.items.indexOf(param);
                if (index > -1) {
                    this.items.splice(index, 1);
                }
            },
            addItem(param){
                this.items.push(param);
            }
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