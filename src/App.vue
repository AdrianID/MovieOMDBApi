<template>
  <div id="app">
    <search @search="changeMovieResult"></search>
  </div>
</template>

<script>
import Search from './components/Search'

export default {
  name: 'app',
  components: {
    Search
  },
  data() {
    return {
      movies: []
    };
  },
  methods: {
    changeMovieResult(results) {
      this.movies = results
    }
  }
};
</script>

