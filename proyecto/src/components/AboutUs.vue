<template>
    <div class="styleAboutMe">
        <h1>{{aboutMe}}</h1>
    </div>
    <div class="formulario">
        <h1>This is my Form:</h1>
        <form action="post" >
            <div class="fieldsForm">
                <input v-model="nameForm" type="text" placeholder="Your name here">
            </div>
            <div class="fieldsForm">
                <input v-model="emailForm" type="email" placeholder="write your email here">
            </div>
            <div class="fieldsForm">
                <textarea v-model="messageForm" placeholder="Send us your comments" rows="8"></textarea>

            </div>
        </form>
        <div class="dataForm">
            <p>Your Name is: {{nameForm}}</p>
            <p>Your email is: {{emailForm}}</p>
            <p>Comments: {{messageForm}}</p>
        </div>
    </div>

</template>

<script>
    export default {
        data() {
            return {
                aboutMe: "Hi I'm Ester!",
                nameForm: "",
                emailForm: "",
                messageForm: "",
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

.formulario{
    margin-top: 15px;
    border: 3px solid blue;
    padding-left: 20px;
    width: 500px;
    background-color: cyan;
}
.dataForm {
    margin-top: 10px;
    font-weight: bold;  
}
.fieldsForm {
    margin-top: 10px;
}

input{
    width: 400px;
}
textarea{
    width: 400px;
}

</style>