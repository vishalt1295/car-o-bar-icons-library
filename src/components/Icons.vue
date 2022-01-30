<template>
  <div class="row">
    <div class="col-md-12 mb-4">
      <h4>Icons</h4>
    </div>
    <ul class="row row-cols-3 row-cols-sm-4 row-cols-lg-6 row-cols-xl-8 list-unstyled list icon-library">
      <li class="col mb-4" v-for="image in images" :key="image">
        <div class="p-3 py-4 mb-2 bg-light text-center rounded">
          <img :src="image" id="image-title" />
        </div>
        <div class="name text-muted text-decoration-none text-center pt-1">
          {{image.slice(5, -13)}}
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  computed: {
    images() {
      const path = require.context("../assets/icons", false, /\.svg$/);
      return path.keys().map(path);
      //console.log(path.keys().map(path))
    },
  },
};
</script>

<style>
.icon-library img {
  width: 3rem;
}
</style>
