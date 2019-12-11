<template>
   <div class="row">
        <div v-for="character in characters.data.results" v-bind:key="character.name" class="col-3">
            {{ character.name }}
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            characters: this.results
        }
    },
    mounted() {
    const axios = require('axios');
        axios
            .get('https://swapi.co/api/people/')
            .then(response => (this.characters = response))
    }
}
</script>