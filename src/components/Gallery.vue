<template>
    <div>
        <b-container class="gallery-container">
            <b-row>
                <b-col><Card 
                v-bind:img="gallery[0].images[0].img" 
                v-bind:alt="gallery[0].images[0].alt"
                v-bind:title="gallery[0].images[0].title" 
                v-bind:subtitle="gallery[0].images[0].subtitle"
                 />
                </b-col>
                <b-col><Card 
                v-bind:img="gallery[0].images[1].img" 
                v-bind:alt="gallery[0].images[1].alt"
                v-bind:title="gallery[0].images[1].title" 
                v-bind:subtitle="gallery[0].images[1].subtitle" />
                </b-col>
            </b-row>
            <b-row>
                <b-col><Card 
                v-bind:img="gallery[1].images[0].img" 
                v-bind:alt="gallery[1].images[0].alt"
                v-bind:title="gallery[1].images[0].title" 
                v-bind:subtitle="gallery[1].images[0].subtitle" /></b-col>
                <b-col><Card 
                v-bind:img="gallery[1].images[1].img" 
                v-bind:alt="gallery[1].images[1].alt"
                v-bind:title="gallery[1].images[1].title" 
                v-bind:subtitle="gallery[1].images[1].subtitle" /></b-col>
            </b-row>
            <b-row>
                <b-col><Card 
                v-bind:img="gallery[2].images[0].img" 
                v-bind:alt="gallery[2].images[0].alt"
                v-bind:title="gallery[2].images[0].title" 
                v-bind:subtitle="gallery[2].images[0].subtitle" /></b-col>
                <b-col><Card 
                v-bind:img="gallery[2].images[1].img" 
                v-bind:alt="gallery[2].images[1].alt"
                v-bind:title="gallery[2].images[1].title" 
                v-bind:subtitle="gallery[2].images[1].subtitle" /></b-col>
            </b-row>
            <b-row>
                <b-col><Card 
                v-bind:img="gallery[3].images[0].img" 
                v-bind:alt="gallery[3].images[0].alt"
                v-bind:title="gallery[3].images[0].title" 
                v-bind:subtitle="gallery[3].images[0].subtitle" /></b-col>
                <b-col><Card 
                v-bind:img="gallery[3].images[1].img" 
                v-bind:alt="gallery[3].images[1].alt"
                v-bind:title="gallery[3].images[1].title" 
                v-bind:subtitle="gallery[3].images[1].subtitle" /></b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
import Vue from "vue";
// Components
import Card from "./Card.vue";
// Gallery Images
import img1 from "../assets/image0.jpeg";
import img2 from "../assets/image2.jpeg";
import img3 from "../assets/img1.png";
import img4 from "../assets/img2.png";
import img5 from "../assets/img9.png";
import img6 from "../assets/img4.png";
import img7 from "../assets/img5.png";
import img8 from "../assets/img6.png";
export default Vue.component("Gallery",{
    components: {
        Card
    },

    data() {
        return {
            gallery: [
        {
          id: 0,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img1,
                  alt: "Image 1",
                  title: "Salt Creek",
                  subtitle: "Port Angeles, WA"
                },
                {
                  id: 1,
                  img: img2,
                  alt: "Image 2",
                  title: "Salt Creek",
                  subtitle: "Port Angeles, WA"
                },
          ]
        },
        {
          id: 1,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img3,
                  alt: "Image 3",
                  title: "Point Defiance Rose Garden",
                  subtitle: "Tacoma, WA"
                },
                {
                  id: 1,
                  img: img4,
                  alt: "Image 4",
                  title: "Lake Crescent",
                  subtitle: "Port Angeles, WA"
                },
          ]
        },
        {
          id: 2,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img5,
                  alt: "Image 5",
                  title: "Point Defiance Rose Garden",
                  subtitle: "Tacoma, WA"
                },
                {
                  id: 1,
                  img: img6,
                  alt: "Image 6",
                  title: "Point Defiance Rose Garden",
                  subtitle: "Tacoma, WA"
                },
          ]
        },
        {
          id: 3,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img7,
                  alt: "Image 7",
                  title: "Lake Crescent",
                  subtitle: "Port Angeles, WA"
                },
                {
                  id: 1,
                  img: img8,
                  alt: "Image 8",
                  title: "Point Defiance Rose Garden",
                  subtitle: "Tacoma, WA"
                },
          ]
        },
      ]
        }
        
    }

})
</script>

<style>
.gallery-container {
    margin-top: 5%;
}

.row {
    margin: 0 0 5% 0 !important;
}
</style>

