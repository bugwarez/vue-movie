<template>
  <div class="wide_carousel_container">
    <h4 class="display-6">Featured Today</h4>
    <n-carousel
      :direction="direction"
      show-arrow
      :dot-type="type"
      :dot-placement="placement"
      :draggable="draggable"
    >
      <n-card class="video_card">
        <template #cover>
          <img
            class="wide_carousel_img p-0 m-0"
            src="../assets/img/content/7801325.jpg"
          />
        </template>
        <h1 class="mt-2 mb-0">The Witcher </h1>
        <div class="d-flex bd-highlight">
          <h5><span class="badge badge-warning ml-2">Action</span></h5>
          <h5><span class="badge badge-warning ml-2">Adventure</span></h5>
          <h5><span class="badge badge-warning ml-2">Drama</span></h5>
        </div>
        <p class="text-light ml-2">
          Geralt of Rivia, a solitary monster hunter, struggles to find his
          place in a world where people often prove more wicked than beasts.
        </p>
      </n-card>
      <n-card class="video_card">
        <template #cover>
          <img
            class="wide_carousel_img"
            src="../assets/img/content/606024.jpg"
          />
        </template>
        <h1 class="mt-2 mb-0">Rick and Morty</h1>
        <div class="d-flex bd-highlight">
          <h5><span class="badge badge-warning ml-2">Animation</span></h5>
          <h5><span class="badge badge-warning ml-2">Adventure</span></h5>
          <h5><span class="badge badge-warning ml-2">Comedy</span></h5>
        </div>
        <p class="text-light ml-2">
          Geralt of Rivia, a solitary monster hunter, struggles to find his
          place in a world where people often prove more wicked than beasts.
        </p>
      </n-card>
      <n-card class="video_card">
        <template #cover>
          <img
            class="wide_carousel_img"
            src="../assets/img/content/breaking_bad_wide.jpg"
          />
        </template>
        <h1 class="mt-2 mb-0">Breaking Bad</h1>
        <div class="d-flex bd-highlight">
          <h5><span class="badge badge-warning ml-2">Crime</span></h5>
          <h5><span class="badge badge-warning ml-2">Drama</span></h5>
          <h5><span class="badge badge-warning ml-2">Thriller</span></h5>
        </div>
        <p class="text-light ml-2">
          Geralt of Rivia, a solitary monster hunter, struggles to find his
          place in a world where people often prove more wicked than beasts.
        </p>
      </n-card>
    </n-carousel>
  </div>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  setup() {
    const typeRef = ref("line");
    const placementRef = ref("bottom");
    const directionRef = ref("horizontal");
    const draggableRef = ref("true");
    return {
      showArrow: ref(true),
      type: typeRef,
      placement: placementRef,
      direction: directionRef,
      draggable: draggableRef,
    };
  },
});
</script>

<style>

@media only screen and (max-width: 480px) {
  .wide_carousel_img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border: 0;
  }
  .wide_carousel_container {
    width: 90%;
    border: 0;
  }
}

@media only screen and (min-width: 1280px) {
  .wide_carousel_img {
    width: 100%;
    height: 500px;
    object-fit: fill;
    /* border: 3px solid gold; */
    border: 0;
  }
  .wide_carousel_container {
    width: 93%;
    border: 0;
  }
}
</style>