<script setup>
import RotatingCard from "../../../examples/cards/rotatingCards/RotatingCard.vue";
import RotatingCardFront from "../../../examples/cards/rotatingCards/RotatingCardFront.vue";
import RotatingCardBack from "../../../examples/cards/rotatingCards/RotatingCardBack.vue";
import DefaultInfoCard from "../../../examples/cards/infoCards/DefaultInfoCard.vue";
</script>
<template>
  <section class="my-5 py-5">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-4 ms-auto me-auto p-lg-4 mt-lg-0 mt-4">
          <RotatingCard>
            <RotatingCardFront
              image="https://images.unsplash.com/photo-1569683795645-b62e50fbf103?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=987&q=80"
              icon="touch_app"
              title="Probleme mit einer App?"
              description="Melde dich doch bei uns und wir können zusammen am Problem arbeiten."
            />

            <RotatingCardBack
              image="https://images.unsplash.com/photo-1498889444388-e67ea62c464b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1365&q=80"
              title="Anmeldung"
              description="Rufe uns an oder komm vorbei."
              :action="[
                {
                  route: './pages/landing-pages/contact-us',
                  label: 'Kontakt',
                },
              ]"
            />
          </RotatingCard>
        </div>
        <div class="col-lg-6 ms-auto">
          <div class="row justify-content-start">
            <DefaultInfoCard
              icon="content_copy"
              title="Lokaler Treffpunkt"
              description="Sie können uns nicht nur telefonisch erreichen, sondern auch durch Hilfe vor Ort.Nicht nur können Sie uns telefonisch erreichen, sonder auch lokal vor ort support vorhanden."
            />
            <DefaultInfoCard
              icon="flip_to_front"
              title="Geschulte Fachkräfte"
              description="Sie können sich darauf verlassen, dass Sie durch unsere Auswahl- und Schulungsprozesse unserer Fachkräfte angemessen unterstützt werden."
            />
          </div>
          <div class="row justify-content-start mt-5">
            <DefaultInfoCard
              class="mt-3"
              icon="price_change"
              title="Zeit und Geld sparen"
              description="Ersparen Sie sich den Gang zu den kostenpflichtigen Hotlines und erwerben Sie stattdessen bei uns neue Fähigkeiten für den Alltag."
            />
            <DefaultInfoCard
              class="mt-3"
              icon="devices"
              title="Online Hilfe"
              description="Wir können auch zusammenarbeiten, um Ihre Probleme über das Internet zu lösen."
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
