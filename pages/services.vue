<template>
    <div>
    <h1>Services View</h1>
    <nav>
      <ul>
        <li>
          <NuxtLink to="/services/marketing">Marketing</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/services/web-design">Web Design</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/services/technical-seo">Technical SEO</NuxtLink>
        </li>
      </ul>
    </nav>
    <NuxtChild  />
  </div>
</template>
<script>
export default {
  transition: "services",
  data() {
    return {
      title: "Services Page",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Services Page Description",
        },
      ],
    };
  },
};
</script>
<style scoped>
ul {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0;
}
li {
  margin: 0 0.5rem;
  padding: 0.25rem;
  font-size: 1rem;
}
.services-enter-active,
.services-leave-active {
  transition: opacity 0.5s;
}
.services-enter,
.services-leave-active {
  opacity: 0;
}
</style>