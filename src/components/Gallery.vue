<template>
    <div>
        <b-container fluid>
            <b-row>
                <b-col><img v-bind:img-src="img1" alt="image 1"></b-col>
                <b-col><img v-bind:img-src="img2" alt="image 2"></b-col>
            </b-row>
            <b-row>
                <b-col><img v-bind:img-src="img3" alt="image 3"></b-col>
                <b-col><img v-bind:img-src="img4" alt="image 4"></b-col>
            </b-row>
            <b-row>
                <b-col><img v-bind:img-src="img5" alt="image 5"></b-col>
                <b-col><img v-bind:img-src="img6" alt="image 6"></b-col>
            </b-row>
            <b-row>
                <b-col><img v-bind:img-src="img7" alt="image 7"></b-col>
                <b-col><img v-bind:img-src="img8" alt="image 8"></b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
import Vue from "vue";
export default Vue.component("Gallery",{
    props: {
    }

})
</script>

<style scoped>
</style>

