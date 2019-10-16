<template>
    <div class="addItem">
        <input type="text" id="addItemInput" placeholder="type..">
        <button id="addItemAction">add</button>
    </div>
</template>

<script>
    export default {
        name: "AddItem"
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