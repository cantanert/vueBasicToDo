<template>
    <div class="addItem">
        <input type="text" id="addItemInput" placeholder="type..." v-model="inputValue" @keyup.enter="addItem">
        <button id="addItemAction" @click="addItem()" >add</button>
    </div>
</template>

<script>
    export default {
        name: "AddItem",
        data(){
            return {
                inputValue : ""
            }
        },
        methods: {
            addItem(){
                if(this.inputValue.length !== 0){
                    this.$emit("add-item",this.inputValue);
                }
            }
        }
    }
</script>

<style scoped>
    .addItem{

    }

    #addItemInput{
        width: 75%;
    }

    #addItemAction{
        width: 25%;
    }
</style>