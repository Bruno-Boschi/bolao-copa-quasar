<template>
  <q-list>
    <!-- DASHBOOARD -->
    <q-item clickable to="/" exact>
      <q-item-section avatar>
        <q-icon name="mdi-view-dashboard" />
      </q-item-section>

      <q-item-section>
        <q-item-label>Dashboard</q-item-label>
      </q-item-section>
    </q-item>
    <!-- FIM DASHBOARD -->

    <!-- MATERIAS -->
    <q-item clickable to="/palpites" exact>
      <q-item-section avatar>
        <q-icon name="mdi-page-next" />
      </q-item-section>

      <q-item-section>
        <q-item-label>Palpites</q-item-label>
      </q-item-section>
    </q-item>

    <q-item clickable to="/ranking" exact>
      <q-item-section avatar>
        <q-icon name="mdi-chart-line" />
      </q-item-section>

      <q-item-section>
        <q-item-label> Ranking </q-item-label>
      </q-item-section>
    </q-item>

    <q-item clickable to="/duvidas" exact>
      <q-item-section avatar>
        <q-icon name="mdi-frequently-asked-questions" />
      </q-item-section>

      <q-item-section>
        <q-item-label>Duvidas</q-item-label>
      </q-item-section>
    </q-item>

    <q-item clickable to="/materias/leilao" exact>
      <q-item-section avatar>
        <q-icon name="mdi-gavel" />
      </q-item-section>

      <q-item-section>
        <q-item-label>Leilão</q-item-label>
      </q-item-section>
    </q-item>

    <!-- <q-item clickable to="/materias/leilao" exact>
      <q-item-section avatar>
        <q-icon name="mdi-gavel" />
      </q-item-section>

      <q-item-section>
        <q-item-label>Leilão</q-item-label>
      </q-item-section>
    </q-item> -->
  </q-list>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "EssentialLink",
  props: {
    title: {
      type: String,
      required: true,
    },

    caption: {
      type: String,
      default: "",
    },

    route: {
      type: String,
      default: "",
    },

    icon: {
      type: String,
      default: "",
    },
  },
});
</script>
