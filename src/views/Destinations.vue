<template>
  <div class="destinations">
    <p>
      {{ id }}
    </p>
    <div v-if="sortDestinationsBy === 'cheapness'">
      <div v-for="destination in origin.origin_trip_destinys">
        <p>{{ destination.name }}</p>
      </div>
    </div>

    <div v-if="sortDestinationsBy === 'mix'">
    </div>
    
    <div v-if="sortDestinationsBy === 'rank'">
      <div v-for="destination in limitBy(orderBy(destinations, 'rank'), 31)">
        <p>{{ destination.name }}</p>
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
      origin: {},
      sortDestinationsBy: ""
    };
  },
  created: function() {
    axios.get("/api/destinations").then(response => {
      this.destinations = response.data;
    });

    this.destinations.forEach(function(destination) {
      if (destination.airport_code === this.$route.query.origin) {
        let i = 0;
        console.log(i);
        this.id = destination.id;
        i += 1;
      }
    });

    console.log(this.id);

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
  },
  methods: {}
};
</script>