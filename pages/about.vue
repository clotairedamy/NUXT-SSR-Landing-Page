<template>
  <div>
    <h1>About Me View</h1>
  </div>
</template>

<script>
export default {
  transition: "about",
  data() {
    return {
      title: "About Page",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "About page description",
        },
      ],
    };
  },
};
</script>
<style>
.about-enter-active,
.about-leave-active {
  transition: opacity 0.5s;
}
.about-enter,
.about-leave-active {
  opacity: 0;
}
</style>
