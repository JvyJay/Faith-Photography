<template>
    <div>
        <b-container>
            <b-row>
                <b-col><img v-bind:img-src="img1"></b-col>
                <b-col><img v-bind:img-src="img2" alt=""></b-col>
            </b-row>
            <b-row>
                <b-col><img v-bind:img-src="img3" alt=""></b-col>
                <b-col><img v-bind:img-src="img4" alt=""></b-col>
            </b-row>
            <b-row>
                <b-col><img v-bind:img-src="img5" alt=""></b-col>
                <b-col><img v-bind:img-src="img6" alt=""></b-col>
            </b-row>
            <b-row>
                <b-col><img v-bind:img-src="img7" alt=""></b-col>
                <b-col><img v-bind:img-src="img8" alt=""></b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
// Gallery Images
import img1 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/image0.jpeg";
import img2 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/image2.jpeg";
import img3 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img1.png";
import img4 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img2.png";
import img5 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img4.png";
import img6 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img5.png";
import img7 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img7.png";
import img8 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img8.png";



export default {
    name: "Gallery",

    data() {
        return {
            img1: img1,
            img2: img2,
            img3: img3,
            img4: img4,
            img5: img5,
            img6: img6,
            img7: img7,
            img8: img8
        }
    }

}
</script>

<style scoped>
    img {
        width: 15% !important;
    }
</style>

