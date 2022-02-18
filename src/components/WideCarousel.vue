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
      <n-card title="Card with Cover">
        <template #cover>
          <img
            class="vertical_carousel_img"
            src="../assets/img/content/1053138.jpg"
          />
        </template>
        Card Content </n-card
      ><n-card title="Card with Cover">
        <template #cover>
          <img
            class="vertical_carousel_img"
            src="../assets/img/content/606024.jpg"
          />
        </template>
        Card Content
      </n-card>
      <n-card title="Card with Cover">
        <template #cover>
          <img
            class="vertical_carousel_img"
            src="../assets/img/content/breaking_bad_wide.jpg"
          />
        </template>
        Card Content
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
  .vertical_carousel_img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  .vertical_carousel_container {
    margin-left: 5vw;
    margin-top: 4vh;
    width: 90%;
  }
}

@media only screen and (max-width: 1920px) {
  .vertical_carousel_img {
    width: 100%;
    height: 420px;
    object-fit: fill;
  }
  .vertical_carousel_container {
    margin-left: 4vw;
    margin-top: 4vh;
    width: 60%;
  }
}
</style>