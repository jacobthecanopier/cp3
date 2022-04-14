<template>
  <div class="wrapper">
    <ReviewsComponent :reviews="reviews" />
  </div>
</template>

<script>
import ReviewsComponent from "../components/ReviewsComponent.vue";

export default {
  name: "ReviewsView",
  components: {
    ReviewsComponent,
  },
  computed: {
    reviews() {
      return this.$root.$data.reviews;
    },
  },
};
</script>
