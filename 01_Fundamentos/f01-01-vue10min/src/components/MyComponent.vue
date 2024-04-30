<template>
    <div class="my-component" style="align-items: center;">
        <h1 v-bind:class="{ highlighted: isHighlighted }" >{{ title }}</h1>
        <button @click="toggleHighlight()">Resaltar: v-bind</button>
        <hr>

        <!-- //Uso de eventos SIN-METODOS
            <button v-on:click="$event => isVisible = !isVisible">Toggle isVisible</button> 
        -->
        <!--//Uso de eventos CON-METODOS-->
        <button v-on:click="toggleVisibility()">Toggle isVisible: v-on</button>
        <!--//v-Model-->&nbsp;
        <input v-model="message">
        <br>
        <div style="display:flex; flex-direction:row; align-items:center">
            <img alt="Vue logo" width="50px" src="..\assets\logo.png">
            <h1 v-if="isVisible">{{ message }}</h1>
        </div>
        <hr>

        <button v-on:click="sayHello()">v-on:click sayHello()</button>
        <br><br>
        Se puede hacer invocación de eventos <b>"v-on"</b>,<br>con la abreviatura de <b>"@"</b>
        &nbsp;<button @click=" sayHello(); ">Hey 2: @</button>
        <hr>
        <ul>
            <li v-for="item in list" :key="item.id" style="text-align: left;">v-for: {{ item.id }},{{ item.text }}</li>
        </ul>
    </div>
</template>

<style>
    .highlighted{
        color: aqua;
        font-weight: bold;
        font-size: 3em;
    }
</style>

<script>
    export default{
        name: 'MyComponent',
        data(){ //Variables de operacion
            return{ 
                message: 'Hola Mundo, VUE!!!' ,
                isVisible: true,
                list:[
                    { id: 1, text: 'Firs item' },
                    { id: 2, text: 'Second item' },
                    { id: 3, text: 'Third item' }
                ],
                title: 'Texto de Título',
                isHighlighted: false
            }
        },
        methods:{
            toggleVisibility(){
                this.isVisible = !this.isVisible;
            },
            sayHello(){
                alert('Hey, Listen!, WATCH OUT!!!');
            },
            toggleHighlight(){
                this.isHighlighted = !this.isHighlighted;
            }
        }
    }
</script>

