<template>
    <div class="about">
        <h1>Code of Conduct</h1>
        <h2>1. Sei nicht nervig</h2>
        <p></p>
        <hr>
        <div v-if="!clicked">
            <p>Wie hilfreich war diese Seite?</p>
            <button v-on:click="clicked=true">Yes</button>
        </div>
        <p v-if="clicked">thank</p>
    </div>
</template>

<script>
    export default {
        data: function() {
            return {
                clicked: false
            }
        }
    }
</script>
