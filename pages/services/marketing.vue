<template>
  <div>
    <h1>Marketing {{ $route.params.slug }}</h1>
  </div>
</template>
<script>
export default {
  transition: "marketing",
  data() {
    return {
      title: "Services Marketing page",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Services Marketing page description",
        },
      ],
    };
  },
};
</script>
<style>
.marketing-enter-active,
.marketing-leave-active {
  transition: opacity 0.5s;
}
.marketing-enter,
.marketing-leave-active {
  opacity: 0;
}
</style>