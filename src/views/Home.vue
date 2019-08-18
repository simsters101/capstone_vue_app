<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <p>Please enter the 3 letter code of your closest major airport:</p>
    <form @submit.prevent="redirectToDestinations()">
      <p><input type="text" v-model="origin" list="airport_code"></p>
      <datalist id="airport_code">
        <option v-for="destination in destinations">{{ destination.airport_code }}</option>
      </datalist>
      <p>Choose one:</p>
        <p><input type="radio" v-model="moneyToSpend" value="budget">I'm on a tight budget</p>
        <p><input type="radio" v-model="moneyToSpend" value="mix">I've got some money to spend</p>
        <p><input type="radio" v-model="moneyToSpend" value="lotsOfMoney">I've got all the money in the world</p>
      <p><input type="submit"></p>
    </form>
  </div>
</template>

<style>
</style>

<script>
import axios from "axios";
import Vue2Filters from "vue2-filters";

export default {
  mixins: [Vue2Filters.mixin],
  data: function() {
    return {
      message: "Welcome to Wanderlust!",
      origin: "",
      destinations: [],
      moneyToSpend: "",
    };
  },
  created: function() {
    axios.get("/api/destinations").then(response => {
      console.log(response.data);
      this.destinations = response.data;
    });
  },
  methods: {
    redirectToDestinations: function() {
      var origin = this.origin;
      var moneyToSpend = this.moneyToSpend;
      this.$router.push({ path: 'destinations', query: { origin, moneyToSpend }});
    }
  }
};
</script>