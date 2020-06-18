<template>
  <div id="app">
<<<<<<< HEAD
    <header class="head">
      <div class="header">
        <div class="container" :class="{ show: showSidebar }">
          <div class="control">
            <i class="fas fa-bars" @click="showNav"></i>
          </div>
        </div>
        <div class="logo">
          <h1>logo</h1>
        </div>
        <div class="icon">
          <i class="fas fa-code"></i>
        </div>
      </div>
    </header>
    <div class="content"></div>
=======
    aaaaaaaaaa
     <GmapMap
  :center="{lat:10, lng:10}"
  :zoom="7"
  map-type-id="terrain"
>
  <GmapMarker
    :key="index"
    v-for="(m, index) in markers"
    :position="m.position"
    :clickable="true"
    :draggable="true"
    @click="center=m.position"
  />
</GmapMap>
>>>>>>> 6fcd4d88c99323695aae2789aa6b1254acb2c1e1
  </div>
</template>
<script>
<<<<<<< HEAD
export default {
  name: "App",
  data: () => {
    return {
      showSidebar: false,
    };
  },
  methods: {
    showNav() {
      this.showSidebar = !this.showSidebar;
    },
  },
};
</script>
=======


import {gmapApi, gmapMarker} from 'vue2-google-maps'

export default {
  name: 'App',
  computed: {
    google: gmapApi
  },
}
</script>
>>>>>>> 6fcd4d88c99323695aae2789aa6b1254acb2c1e1
