<template>
    <div>
        <b-card
            v-bind:img-src="img"
            v-bind:img-alt="alt"
            text-variant="black"
            v-bind:title="title"
            v-bind:sub-title="subtitle"
        >
        </b-card>
    </div>
</template>

<script>
import Vue from "vue";

export default Vue.component("Card", {
    props: {
        img: String,
        alt: String,
        title: String,
        subtitle: String
    }
})
</script>

<style scoped>

</style>
