<script setup>
import { onMounted } from "vue";

// Sections components
import BaseLayout from "./components/BaseLayout.vue";
import View from "./components/View.vue";

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
    title="Bild versenden"
    :breadcrumb="[{ label: 'Grundlagen', route: '#' }, { label: 'Bild versenden' }]"
  >

  <div class="container">
<div class="row">
  <div class="col">
<span><h3>Schritt 1</h3>
Zuerst musst du die Person auswählen zu welchem du ein Bild senden willst. <hr></span>
  </div>
  <div class="col">
<span><h3>Schritt 2</h3>
 Drücke auf die Kamera unten rechts vom Bildschirm und wähle ein Bild aus. <hr> </span>
  </div>
  <div class="col">
<span><h3>Schritt 3</h3>
  Dannach wählst du das Bild aus welches du versenden willst. <hr> </span>
  </div>
</div>
<div class="row">
  <div class="col">
    <span><img width="300" src="https://i.imgur.com/GE883ve.jpg"></span>
  </div>
  <div class="col">
    <span><img width="300" src="https://i.imgur.com/nYO0W3U.jpg"></span>
  </div>
  <div class="col">
    <span><img width="300" src="https://i.imgur.com/M7AxEn0.jpg"></span>
  </div>
</div>
</div>

  </BaseLayout>
</template>
