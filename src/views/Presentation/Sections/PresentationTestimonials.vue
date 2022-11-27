<script setup>
import DefaultReviewCard from "@/examples/cards/reviewCards/DefaultReviewCard.vue";
</script>
<template>
  <section class="py-7">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 mx-auto text-center">
          <h2 class="mb-0">Vertrauen von über</h2>
          <h2 class="text-gradient text-success mb-3">
            1'000+ Nutzer
          </h2>
          <p class="lead">
            Mehr als 1.000 Personen haben unsere Hilfe in Anspruch genommen, und sie alle konnten sich mit unserer Unterstützung neue Technologien aneignen.
          </p>
        </div>
      </div>
      <div class="row mt-6">
        <DefaultReviewCard
          name="Nick Willever"
          date="1 day ago"
          review='"Dies ist ein hervorragendes Produkt, der Serice ist ausgezeichnet 
          und hat mir geholfen, Dinge effizienter zu erledigen."'
          :rating="5.0"
        />
        <DefaultReviewCard
          class="ms-md-auto"
          color="bg-gradient-success"
          name="Shailesh Kushwaha"
          date="1 week ago"
          review='"Ich habe bei Zenior die Lösung für alle meine
           technischen Bedürfnisse gefunden. Und es ist wirklich 
           erschwinglich, sehr bescheiden Jungs !!!"'
          :rating="5.0"
        />

        <DefaultReviewCard
          name="Samuel Kamuli"
          date="3 weeks ago"
          review='"Toller
           Service."'
          :rating="5.0"
        />
      </div>
    </div>
  </section>
</template>
