<template>
  <div id="app">
    asd
    <Header />
    <MemoApp />
  </div>
</template>

<script>
import Header from "./components/AppHeader";
import MemoApp from "./components/MemoApp";
export default {
  name: "app",
  components: {
    Header,
    MemoApp
  }
};
</script>

<style>
@import "/style.reset.css";
#app {
  width: 560px;
  margin: 0 auto;
}
</style>
