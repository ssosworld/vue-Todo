<template>
    <div class="clearAllContainer">
        <span class="clearAllbtn" @click="clearTodo">Clear ALl</span>

    </div>
</template>




<script>
export default {
    methods: {
        clearTodo(){
            //localStorage.clear();
            this.$emit('removeAll');
        }
    }
    
}
</script>

<style scoped>
    .clearAllContainer{
        width: 8.5rem;
        height: 50px;
        line-height: 50px;
        background-color: white;
        border-radius: 5px;
        margin: 0 auto;
    }
    .clearAllbtn{
        color: #e20303;
        display: black;
    }

</style>


