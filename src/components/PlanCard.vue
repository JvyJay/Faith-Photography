<template>
    <div class="plan-card">
        <b-card class="mx-auto"
            v-bind:img-src="img"
            v-bind:img-alt="alt"
            text-variant="black"
            v-bind:title="title"
            v-bind:sub-title="subtitle"

        >
        <ul>
            <li>{{ bulletpoint1 }}</li>
            <li>{{ bulletpoint2 }}</li>
            <li>{{ bulletpoint3 }}</li>
        </ul>
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
        desc: String,
        bulletpoint1: String,
        bulletpoint2: String,
        bulletpoint3: String
    }
})
</script>

<style scoped>
.plan-card {
    margin: 10px;
}

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