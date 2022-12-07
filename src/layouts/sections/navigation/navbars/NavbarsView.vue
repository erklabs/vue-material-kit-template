<script setup>
import { onMounted } from "vue";

// Sections components
import BaseLayout from "../../components/BaseLayout.vue";
import View from "../../components/View.vue";

// Navbars page components
import NavbarDark from "./components/NavbarDark.vue";

// Navbars page components codes
import { navbarDarkCode } from "./components/codes";

//nav-pills
import setNavPills from "@/assets/js/nav-pills";

import TransparentBlogCard from "@/examples/cards/blogCards/TransparentBlogCard.vue";

//hook
onMounted(() => {
  setNavPills();
});
</script>
<template>
  <BaseLayout
    title="Grundlagen"
    :breadcrumb="[{ label: 'Grundlagen', route: '#' }, { label: 'Grundlagen' }]"
  >

 <div class="container">
<div class="row">
  <div class="col-sm">
    <TransparentBlogCard
  image="https://images.unsplash.com/photo-1519069060891-f8c50519bf39?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&h=300&w=450&q=80"
  title="Bild versenden"
  description="Hier kannst du nachschauen wie du Bilder versenden kannst ..."
  :action="{
    label: 'Mehr lesen',
    route: '/bildVersenden',
    color: 'success',
  }"
 />
  </div>
  <div class="col-sm">
    <TransparentBlogCard
  image="https://images.unsplash.com/photo-1557200134-90327ee9fafa?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&h=300&w=450&q=80"
  title="Email versenden"
  description="Hier kannst du nachschauen wie du Emails versenden kannst ..."
  :action="{
    label: 'Mehr lesen',
    route: '/',
    color: 'success',
  }"
 />
  </div>
  <div class="col-sm">
    <TransparentBlogCard
  image="https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&h=300&w=450&q=80"
  title="Soziale Medien"
  description="Erfahre mehr über Soziale Medien ..."
  :action="{
    label: 'Mehr lesen',
    route: '/',
    color: 'success',
  }"
 />
  </div>
</div>
</div>


  </BaseLayout>
</template>
