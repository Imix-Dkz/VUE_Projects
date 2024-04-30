<template>
    <div id="app">
        <h1>{{ message2 }}</h1>
        <button @click="changeMessage()">{{ message2 }}</button>
    </div>
</template>
<script>
    import { mapState, mapMutations } from 'vuex';
    export default {
        computed: {
            ...mapState(['message2'])
        },
        methods: {
            ...mapMutations(['setMessage']),
            changeMessage() {
                this.setMessage('Hello from MyComponent2');
            }
        }
    }
</script>