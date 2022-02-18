<template>
  <div class="home">
    <div class="row p-0 m-0 ml-5 mt-3">
      <div class="col-8">
        <WideCarousel />
      </div>
      <div class="col text-start">
        <MostViewedCard />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import WideCarousel from "@/components/WideCarousel";
import MostViewedCard from "@/components/MostViewedCard";
export default {
  components: {
    WideCarousel,
    MostViewedCard,
  },
};
</script>
<style lang="scss">
</style>
