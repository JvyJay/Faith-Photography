<template>
    <div>
        <b-card class="mx-auto"
            v-bind:img-src="img"
            v-bind:img-alt="alt"
            text-variant="black"
            v-bind:title="title"
            v-bind:sub-title="subtitle"

        >
        <router-link to="/contact"><b-button pill>Contact</b-button></router-link>
        </b-card>
    </div>
</template>

<script>
import Vue from "vue";

export default Vue.component("PlanCard", {
    name: "PlanCard",
    props: {
        img: String,
        alt: String,
        title: String,
        subtitle: String,
        desc: String
    }
})
</script>

<style scoped>
.card-img {
  width: 20% !important;
}

.card {
    justify-content: center !important;
    align-items: center !important;
}

.btn {
  color: rgb(255, 149, 220);
  border-color: rgb(255, 149, 220);
}

.btn-secondary {
  color: rgb(255, 149, 220);
  background-color: #fff;
  border-color: rgb(255, 149, 220);
}

.btn:hover {
    color: #fff;
    background-color: rgb(255, 149, 220);
    transition: ease-in-out 0.1s;
}

a {
    color: rgb(255, 149, 220);
}

a:hover {
    color: #fff;
}
</style>