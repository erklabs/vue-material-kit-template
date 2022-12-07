<script>
import TransparentBlogCard from "@/examples/cards/blogCards/TransparentBlogCard.vue";
</script>
<template>
  <div class="container position-sticky z-index-sticky top-0">
    <div class="row">
      <div class="col-sm">
        <TransparentBlogCard
          image="https://bit.ly/3HH2M6E"
          title="MateLabs mixes machine learning with IFTTT"
          description="If you’ve ever wanted to train a machine learning model and integrate it with IFTTT, you now can with ..."
          :action="{
            label: 'Read more',
            route: '/',
            color: 'success',
          }"
        />
      </div>
      <div class="col-sm">
        <TransparentBlogCard
          image="https://bit.ly/3HH2M6E"
          title="MateLabs mixes machine learning with IFTTT"
          description="If you’ve ever wanted to train a machine learning model and integrate it with IFTTT, you now can with ..."
          :action="{
            label: 'Read more',
            route: '/',
            color: 'success',
          }"
        />
      </div>
      <div class="col-sm">
        <TransparentBlogCard
          image="https://bit.ly/3HH2M6E"
          title="MateLabs mixes machine learning with IFTTT"
          description="If you’ve ever wanted to train a machine learning model and integrate it with IFTTT, you now can with ..."
          :action="{
            label: 'Read more',
            route: '/',
            color: 'success',
          }"
        />
      </div>
    </div>
  </div>
</template>

<style></style>
