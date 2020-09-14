<template>
    <div>
        <h1>Web Design View</h1>
    </div>
</template>
<script>
export default {
  transition: "webdesign",
  data() {
    return {
      title: "Webdesign page",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Services Web Design page description",
        },
      ],
    };
  },
};
</script>
<style>
.webdesign-enter-active,
.webdesign-leave-active {
  transition: opacity 0.5s;
}
.webdesign-enter,
.webdesign-leave-active {
  opacity: 0;
}
</style>