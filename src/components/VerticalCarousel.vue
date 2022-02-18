<template>
  <div class="vertical_carousel_container">
    <n-carousel
      autoplay
      :direction="direction"
      show-arrow
      :dot-type="type"
      :dot-placement="placement"
      :draggable="draggable"
    >
      <img
        class="vertical_carousel_img"
        src="https://m.media-amazon.com/images/M/MV5BOThjODMyM2QtNTNhYi00ZGM4LWIxZTAtMDAyYWNhYzYxMjJiXkEyXkFqcGdeQXVyMTMzNDExODE5._V1_FMjpg_UX968_.jpg"
      />
      <img
        class="vertical_carousel_img"
        src="https://m.media-amazon.com/images/M/MV5BYTRiNDQwYzAtMzVlZS00NTI5LWJjYjUtMzkwNTUzMWMxZTllXkEyXkFqcGdeQXVyNDIzMzcwNjc@._V1_FMjpg_UX1102_.jpg"
      />
      <img
        class="vertical_carousel_img"
        src="https://m.media-amazon.com/images/M/MV5BZGQ2YmMxZmEtYjI5OS00NzlkLTlkNTEtYWMyMzkyMzc2MDU5XkEyXkFqcGdeQXVyMzQ2MDI5NjU@._V1_FMjpg_UY720_.jpg"
      />
      <img
        class="vertical_carousel_img"
        src="https://m.media-amazon.com/images/M/MV5BZjRjOTFkOTktZWUzMi00YzMyLThkMmYtMjEwNmQyNzliYTNmXkEyXkFqcGdeQXVyNzQ1ODk3MTQ@._V1_FMjpg_UY720_.jpg"
      />
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
.vertical_carousel_img {
  width: 100%;
  height: 65vh;
  object-fit: cover;
}
.vertical_carousel_container {
  margin-left: 5vw;
  margin-top: 4vh;
  width: 25%;
}
</style>