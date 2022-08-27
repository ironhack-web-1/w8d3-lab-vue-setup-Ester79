<template>
    <div class="styleAboutMe">
        <h1>{{aboutMe}}</h1>

    </div>
</template>

<script>
    export default {
        data() {
            return {
                aboutMe: "Hi I'm Ester!"
            };
        },        
    }
</script>

<style scoped>
.styleAboutMe {
    color: blue;
    font-family:Arial, Helvetica, sans-serif;
    border: 3px solid darkblue;
    background-color: greenyellow;
    width: fit-content;
    padding: 0px 25px 0px 25px;   
}
.styleAboutMe:hover{
    background-color: aqua;
    color: white;
    width:50%;
    padding-left: 40%;
    margin-left: auto;
    margin-right: auto;   
}

</style>