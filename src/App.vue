<template>
  <COB-Icons />
</template>

<script>
import COBIcons from "./components/COB-Icons.vue";
import "./css/Car-O-Bar-Icons-V3.css";

export default {
  name: "App",
  components: {
    COBIcons,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  /*text-align: center;
  /*color: #2c3e50;
  /*margin-top: 60px;*/
}

@media (prefers-color-scheme: dark) {
  #app {
    background: #212529;
    color: white;
  }
  .icon-demo {
    border: 1px solid #343a40 !important;
  }
  .highlight {
    background: #343a40 !important;
  }
  .icon-titles {
    color: #ced4da !important;
  }
}
</style>
