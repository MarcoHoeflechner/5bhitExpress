<template>
    <div>
        <div id="header">
            <img src ="../assets/htlwels.png"/>
        </div>
        <div id="error" v-if="errorMessage !=''">
            <h3>!! Hinweis !!</h3>
            {{ errorMessage}}
        </div>
    </div>
</template>

<script>
export default {
    props: {
        errorMessage: {
            type: String,
            required:false,
            default:''
        }
    }
}
</script>

<style scoped>
#header {
    display: flex;
    flex-wrap: wrap;
    align-items:baseline;
    justify-content: center;
    margin-top:0px;
    
}
#header h2 {
    margin-left: 10px;
    margin-right: 10px;
}


#error {
    color: red;
}
#error h3 {
    margin:0;
    color:black;
}
</style>