<template>
    <div>
        <p>Serves Status: {{ status }}</p>
        <hr>
        <button @click="changeStatus">Change status</button>
    </div>
</template>

<script>
export default {
    data: function(){
        return{
            status: 'critical'
        }
    },
    methods: {
        changeStatus(){
            this.status= 'Normal'
        }
    }
}
</script>

<style lang="scss">
    button{
        padding:5px;
        border-radius: 0;
        background-color: lightseagreen;
        color:#ffffff;
    }
</style>