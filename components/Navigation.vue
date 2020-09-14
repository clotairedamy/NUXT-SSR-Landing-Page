<template>
  <nav>
    <ul>
      <li>
        <NuxtLink to="/">home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/about">about</NuxtLink>
      </li>
         <li>
        <NuxtLink to="/services">services</NuxtLink>
      </li>
         <li>
        <NuxtLink to="/contact">get in touch</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
nav {
  padding: 0 1rem;
}

ul {
  list-style-type: none;
  padding: 0;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

li {
  margin: 0 0.5rem;
  padding: 0.25rem;
  font-size: 1.2rem;
}
</style>