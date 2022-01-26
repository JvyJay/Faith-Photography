<template>
  <div class="service">
      <h1>Services</h1>
      <b-container >
        <b-row>
            <b-col>
              <PlanCard 
              v-bind:id="cardObj[0].id"
              v-bind:title="cardObj[0].title"
              v-bind:subtitle="cardObj[0].subtitle"
              v-bind:img="cardObj[0].img"
              v-bind:alt="cardObj[0].alt"
              v-bind:bulletpoint1="cardObj[0].bulletpoint1"
              v-bind:bulletpoint2="cardObj[0].bulletpoint2"
              v-bind:bulletpoint3="cardObj[0].bulletpoint3" />
            </b-col>
            <b-col>
              <PlanCard
              v-bind:id="cardObj[1].id"
              v-bind:title="cardObj[1].title"
              v-bind:subtitle="cardObj[1].subtitle"
              v-bind:img="cardObj[1].img"
              v-bind:alt="cardObj[1].alt"
              v-bind:bulletpoint1="cardObj[1].bulletpoint1"
              v-bind:bulletpoint2="cardObj[1].bulletpoint2"
              v-bind:bulletpoint3="cardObj[1].bulletpoint3" />
            </b-col>
        </b-row>
        <p>To book a consultation please Email or direct message me on instagram with your full name, the package you are interested in and where you are located! I’m so excited to create with you !</p>
        <div class="footer">
        <footer>Copyright © Faith Photography 2022</footer>
      </div>
      </b-container>
  </div>
</template>

<script>
// Components
import PlanCard from "../components/PlanCard.vue";

// Images
import basic from "../assets/basic-plan.png";
import premium from "../assets/premium-plan.png";

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
          subtitle: "$100/Session",
          img: basic,
          alt: "Basic Plan Icon",
          bulletpoint1: "1 Hours",
          bulletpoint2: "20 Digital Images",
          bulletpoint3: "1 Location"
        },
        {
          id: 1,
          title: "Premium Package",
          subtitle: "$175/Session",
          img: premium,
          alt: "Premium Plan Icon",
          bulletpoint1: "2 Hours",
          bulletpoint2: "40 Digital Images",
          bulletpoint3: "2 Locations"
        }
      ]
    }
  }
}
</script>

<style scoped>
footer {
    position: relative;
    padding: 50px;
    bottom: 0;
  }
</style>