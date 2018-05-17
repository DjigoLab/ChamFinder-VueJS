<template>
  <div id="app">
    <AppHeader></AppHeader>
    <router-view/>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader";
export default {
  components: { AppHeader },
  name: "App"
};
</script>

<style>
body {
  padding: 0px;
  margin: 0px;
}
html,
body,
#app {
  min-height: 100%;
}
#app {
    font-family: "Tillana", cursive;

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #212121;
  background: #8bc34a;
}
</style>
