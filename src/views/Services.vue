<template>
  <div class="service">
      <h1>Services</h1>
      <b-container fluid>
        <b-row>
            <b-col>
              <PlanCard 
              v-bind:id="cardObj[0].id"
              v-bind:title="cardObj[0].title"
              v-bind:subtitle="cardObj[0].subtitle"
              v-bind:img="cardObj[0].img"
              v-bind:alt="cardObj[0].alt" />
            </b-col>
            <b-col>
              <PlanCard
              v-bind:id="cardObj[1].id"
              v-bind:title="cardObj[1].title"
              v-bind:subtitle="cardObj[1].subtitle"
              v-bind:img="cardObj[1].img"
              v-bind:alt="cardObj[1].alt" />
            </b-col>
        </b-row>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis optio voluptatem possimus fugit labore quasi dolores distinctio nemo quibusdam sint? Beatae dignissimos eaque modi eos deleniti fuga temporibus voluptate illo quaerat a quae, totam similique, voluptas vero, autem exercitationem sequi non tenetur voluptatum deserunt blanditiis ipsa molestiae. Blanditiis, est architecto.</p>
      </b-container>
      <div class="footer">
        <footer>Copyright © Faith Photography 2022</footer>
      </div>
  </div>
</template>

<script>
// Components
import PlanCard from "../components/PlanCard.vue";

// Images
import basic from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/src/assets/basic-plan.png";
import premium from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/src/assets/premium-plan.png";

export default {
  name: 'Services',
  components: {
    PlanCard
  },
  data(){
    return {
      cardObj: [
        {
          id: 0,
          title: "Basic Package",
          subtitle: "$15/hr",
          img: basic,
          alt: "Basic Plan Icon",
          Desc: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aspernatur recusandae corporis aperiam, natus saepe aliquid porro cumque harum officia vel qui voluptate commodi, sint aliquam! Esse cupiditate illo modi harum, molestiae, similique fuga suscipit quis in architecto odit doloremque"
        },
        {
          id: 1,
          title: "Premium Package",
          subtitle: "$30/hr",
          img: premium,
          alt: "Premium Plan Icon",
          Desc: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aspernatur recusandae corporis aperiam, natus saepe aliquid porro cumque harum officia vel qui voluptate commodi, sint aliquam! Esse cupiditate illo modi harum, molestiae, similique fuga suscipit quis in architecto odit doloremque"
        }
      ]
    }
  }
}
</script>

<style scoped>
footer {
    position: absolute;
    padding: 50px;
    bottom: 0;
  }
</style>