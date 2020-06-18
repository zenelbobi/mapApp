<template>
  <div id="app">
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
  </div>
</template>
<script>
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
