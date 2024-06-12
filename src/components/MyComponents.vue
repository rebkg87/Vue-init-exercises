<!--Componentes*-->

<!-- <template>
    <div id="app">
    <h1>{{ message }}</h1>
</div>
</template>-->

<!--Directivas*-->

<!--<template>
    <div id="app">
        <h1 v-if="isVisible">{{ message }}</h1>
        <p><input v-model="message"></p>
        <button v-on:click="$event => isVisible = !isVisible">Text Visibility</button>
    </div>
</template>-->

<!--Metodos*-->

<template>
    <div id="app">
        <h1 v-if="isVisible">{{ message }}</h1>
        <p><input v-model="message"></p>
        <button v-on:click="textVisibility">Text Visibility</button>
    </div>

</template>

<!--Componentes y Directivas*-->
<!--
<script>
    export default {
        name: 'MyComponents',
        data () {
            return {
                message: '¡Este es un ejemplo de Vue!',
                isVisible: true
            }
        }
    }
</script>
-->

<!--Metodos*-->

<script>
    export default {
        name: 'MyComponents',
        data () {
            return {
                message: '¡Este es un ejemplo de Vue!',
                isVisible: true
            }
        },
        methods: {
            textVisibility() {
                this.isVisible = !this.isVisible
            }
        }
    }
</script>