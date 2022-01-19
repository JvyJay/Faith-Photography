<template>
    <div>
        <b-card
            v-bind:img-src="img"
            v-bind:img-alt="alt"
            text-variant="black"
            title="Image Overlay"
            sub-title="Subtitle"
        >
            <b-card-text>
            Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
        </b-card>
    </div>
</template>

<script>
import Vue from "vue";

export default Vue.component("Card", {
    props: {
        img: String,
        alt: String
    }
})
</script>

<style scoped>

</style>
