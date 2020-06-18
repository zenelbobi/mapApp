<template>
  <div id="app">
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
  </div>
</template>

<script>


import {gmapApi, gmapMarker} from 'vue2-google-maps'

export default {
  name: 'App',
  computed: {
    google: gmapApi
  },
}
</script>