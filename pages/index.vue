<template>
  <div>
    <h1>Home Page View</h1>
  </div>
</template>
<script>
export default {
  transition: "home",
  mode: "out-in",
  data() {
    return {
      title: "Home page",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Home page description",
        },
      ],
    };
  },
};
</script>
<style>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.5s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}
</style>

