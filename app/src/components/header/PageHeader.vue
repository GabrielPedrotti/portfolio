<template>
  <header class="page-header">
    <div class="container">
      <ul class="page-header__content">
        <li>
          <h1 class="page-header__title">putLogo</h1>
        </li>
        <li v-for="item in options" :key="item.id">
          <h1 class="page-header__title">{{ item.title }}</h1>
          <!-- <router-link :to="item.link">{{ item.title }}</router-link> -->
        </li>
      </ul>
    </div>
  </header>
</template>

<script setup>
import { computed } from "vue";
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
  background-color: #1D1D1F;
  border-bottom: 1px solid #ebebeb;
  position: fixed;
  top: 0;
  z-index: 100;
  display: flex;
  width: 100%;
  border: solid 2px red;
}

.page-header__content {
  display: flex;
  align-items: center;
  justify-content: center;
  list-style: none;
}

.page-header__title {
  font-size: 1rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
  padding: 0.5rem;
  color: #F5F5F7;
}

.page-header__description {
  font-size: 0.875rem;
  color: #F5F5F7;
  margin-bottom: 0;
}

</style>
