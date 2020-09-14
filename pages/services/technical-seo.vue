<template>
  <div>
    <h1>Technical SEO View</h1>
  </div>
</template>
<script>
export default {
  transition: "technicalseo",
  data() {
    return {
      title: "Technical SEO page",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Services Technical SEO page description",
        },
      ],
    };
  },
};
</script>
<style>
.technicalseo-enter-active,
.technicalseo-leave-active {
  transition: opacity 0.5s;
}
.technicalseo-enter,
.technicalseo-leave-active {
  opacity: 0;
}
</style>