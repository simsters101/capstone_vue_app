<template>
  <div class="destinations">
    <p>Id: {{ id }}</p>
    <p>{{ origin.name }} ({{ origin.airport_code }})</p>
    <p>Country: {{ origin.country }}</p>
    <p>Continent: {{ origin.continent }}</p>
    <div v-if="sortDestinationsBy === 'cheapness'">
      <p>{{ origin.origin_trip_destinys.length }} destinations to go to</p>
      <br>
      <p>These destinations are listed in order of how much they cost to get to from {{ origin.name }} ({{ origin.airport_code }})</p>
      <hr>
      <div v-for="destination in orderBy(origin.origin_trip_destinys, 'origin_trip.price')">
        <p>{{ destination.destiny.name }}, {{destination.destiny.country}}</p>
        <p>${{ destination.origin_trip.price }}</p>
        <br>
      </div>
    </div>

    <div v-if="sortDestinationsBy === 'mix'">
      <p>This feature is under development. Check back later</p>
    </div>
    
    <div v-if="sortDestinationsBy === 'rank'">
      <hr>
      <div v-for="destination in limitBy(orderBy(destinations, 'rank'), 40)">
        <p>{{ destination.name }}, {{ destination.country }}</p>
      </div>
    </div>
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
      destinations: [],
      id: 221,
      origin: {
        origin_trip_destinys: []
      },
      sortDestinationsBy: "",
    };
  },
  created: function() {
    axios.get("/api/destinations").then(response => {

      this.destinations = response.data;

      this.destinations.forEach((destination) => {
        if (this.$route.query.origin === destination.airport_code) {
          this.id = destination.id;
        }
      });

      axios.get("/api/destinations/" + this.id).then(response => {
        console.log(response.data);
        this.origin = response.data;
      });

      if (this.$route.query.moneyToSpend === 'lotsOfMoney') {
        this.sortDestinationsBy = 'rank';
      } else if (this.$route.query.moneyToSpend === 'budget') {
        this.sortDestinationsBy = 'cheapness';
      } else if (this.$route.query.moneyToSpend === 'mix') {
        this.sortDestinationsBy = 'mix';
      }
    });
  },
  methods: {}
};
</script>