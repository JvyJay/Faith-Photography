<template>
    <div>
        <b-card no-body class="overflow-hidden mx-auto" style="max-width: 1000px;">
    <b-row no-gutters>
      <b-col>
        <b-card-img :src="img" :alt="alt" class="rounded-1"></b-card-img>
      </b-col>
      <b-col>
        <b-card-body title="Horizontal Card">
          <b-card-text>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aspernatur recusandae corporis aperiam, natus saepe aliquid porro cumque harum officia vel qui voluptate commodi, sint aliquam! Esse cupiditate illo modi harum, molestiae, similique fuga suscipit quis in architecto odit doloremque sapiente qui. Ab eum architecto placeat eveniet eaque fugit saepe iure aliquam repellat dolorem, repellendus maxime quisquam rerum laboriosam facilis, ducimus quae corporis unde! Ducimus quae dolorem cupiditate dolor ipsum maxime possimus quibusdam eos amet optio, facilis assumenda aliquam, suscipit veniam.
          </b-card-text>
        </b-card-body>
      </b-col>
    </b-row>
  </b-card>
    </div>
</template>

<script>
import Vue from 'vue';

import img from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/src/assets/about-photo.jpeg"

export default Vue.component("AboutCard",{
    name: "AboutCard",
    data() {
        return {
            img: img,
            alt: "About Image"
        }
    }
})
</script>
