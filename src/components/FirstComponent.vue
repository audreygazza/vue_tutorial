<template>
    <div>
        <h1>Titre 1</h1>
        <h2>Titre 2</h2>
        <p>Message : {{ msg }}</p>
        <p>Seulement premier mot : {{ onlyFirstWord }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            msg: "Hello World"

        }
    },
    computed: {
        onlyFirstWord(){
            return this.msg.split('')[0].toUpperCase();
        }
    },
    
}
</script>

<style>

</style>
