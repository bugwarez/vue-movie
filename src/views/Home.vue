<template>
  <div class="home">
    <div class="feature-card">
      <router-link to="/title/tt0903747">
        <img class="featured-img" src="https://m.media-amazon.com/images/M/MV5BOThjODMyM2QtNTNhYi00ZGM4LWIxZTAtMDAyYWNhYzYxMjJiXkEyXkFqcGdeQXVyMTMzNDExODE5._V1_FMjpg_UX968_.jpg" alt="Breaking Bad">
        <div class="detail">
          <h3>Breaking Bad</h3>
          <p>A high school chemistry teacher diagnosed with inoperable lung cancer turns to manufacturing and selling methamphetamine in order to secure his family's future.</p>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
}
</script>
<style lang="scss">
.home {
  .feature-card {
    position: relative;
    .featured-img {
      display: block;
      width: 100%;
      height: 300px;
      object-fit: cover;
      position: relative;
      z-index: 0;
    }
    .detail {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: rgba(0, 0, 0, 0.6);
      padding: 16px;
      z-index: 1;
    }
  }
}
</style>
