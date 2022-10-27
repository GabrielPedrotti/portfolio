<template>
  <header class="page-header">
    <ul class="page-header-content">
      <li>
        <a class="logo-img" href="/">
          <font-awesome-icon icon="fa-file-code" />
        </a>
      </li>
      <li v-for="item in options" :key="item.id">
        <a :href="item.link">
          <h1 class="page-header-title">{{ item.title }}</h1>
        </a>
        <!-- <router-link :to="item.link">{{ item.title }}</router-link> -->
      </li>
    </ul>
  </header>
</template>

<script setup>
import { computed } from "vue";

const asdasd = computed(() => {
  return "computed value";
});

const options = [
  {
    id: 1,
    title: "Home",
    link: "/",
  },
  {
    id: 2,
    title: "About",
    link: "/about",
  },
  {
    id: 3,
    title: "Contact",
    link: "/contact",
  },
];
</script>

<style>
/* center page-header */
.page-header {
  background-color: #000000cc;
  border-bottom: 1px solid #ebebeb;
  position: fixed;
  top: 0;
  z-index: 9999;
  display: block;
  width: 100%;
}

.page-header-content {
  display: flex;
  align-items: center;
  justify-content: center;
  list-style: none;
  padding: 0;
}

.page-header-title {
  font-size: 15px;
  font-weight: 700;
  padding: 0.8rem;
  color: #f5f5f7;
}

.page-header-title:hover {
  color: #d6d6d6;
}

.logo-img {
  margin: 0.8rem;
  font-size: 1.5rem;
  color: #f5f5f7;
}

.logo-img:hover {
  color: #d6d6d6;
}
</style>
