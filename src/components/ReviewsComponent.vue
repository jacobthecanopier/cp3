<template>
  <div class="experience-container">
    <div class="reviews">
      <div
        class="company-container review"
        v-for="review in reviews"
        :key="review.id"
      >
        <div class="about-me-text review">
          <div class="about-me-title">
            {{ review.name }}
          </div>
          <hr />
          <div class="company-duration">"{{ review.review }}"</div>
          <hr />
          <div class="about-me-reviwer">- {{ review.date }}</div>
        </div>
        <!-- <div>
          <img class="company-icon" :src="'../assets/' + review.photo" />
          <img class="company-icon" src="../assets/john.png" />
        </div> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ReviewsComponent",
  props: {
    reviews: Array,
  },
};
</script>
