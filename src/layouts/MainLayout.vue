<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-btn flat dense round aria-label="Menu" @click="toggleLeftDrawer">
          <q-avatar size="30px">
            <img src="../assets/logo.png" />
          </q-avatar>
        </q-btn>

        <q-toolbar-title>
          <q-img
            class="q-mx-xs"
            src="../assets/logo_text.png"
            style="height: 36px; max-width: 152px"
          />
        </q-toolbar-title>
        <q-btn dense flat round icon="mdi-bell" class="q-mx-md" />
        <q-btn dense flat round class="q-mr-md" @click="toggleRightDrawer">
          <q-avatar size="30px">
            <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
          </q-avatar>
        </q-btn>
      </q-toolbar>
    </q-header>

    <q-drawer
      class="bg-drawer-l text-secondary"
      v-model="leftDrawerOpen"
      show-if-above
    >
      <q-list class="q-mt-md">
        <!-- <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        /> -->
        <EssentialLink />
      </q-list>
      <div
        class="fixed-bottom text-center q-pb-sm text-weight-bold text-teal-8"
      >
        © JOIN ADS
      </div>
    </q-drawer>

    <q-drawer
      class="bg-drawer-l text-secondary"
      v-model="rightDrawerOpen"
      side="right"
      elevated
    >
      <q-img
        class="absolute-top"
        src="https://cdn.quasar.dev/img/material.png"
        style="height: 150px"
      >
        <div class="absolute-bottom bg-transparent">
          <q-avatar size="56px" class="q-mb-sm">
            <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
          </q-avatar>
          <div class="text-weight-bold">Administrador</div>
          <div>Admin@admin</div>
        </div>
      </q-img>
    </q-drawer>

    <q-page-container class="bg-teal-1">
      <router-view />
    </q-page-container>

    <!-- <q-footer class="bg-teal-2 text-black">
      <q-toolbar>
        <q-toolbar-title>
          <div class="text-center text-subtitle2">
            All Rights Reserved by Redação CDD.
          </div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer> -->
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";
import EssentialLink from "src/components/EssentialLink.vue";

const linksList = [
  {
    title: "Dashboard",
    icon: "mdi-view-dashboard",
    route: { nome: "home" },
  },
  {
    title: "Matérias",
    icon: "mdi-post",
  },
  {
    title: "Financeiro",
    icon: "mdi-cash",
  },

  {
    title: "Suporte",
    icon: "mdi-face-agent",
  },

  {
    title: "Usuario",
    icon: "mdi-account-group",
  },
  {
    title: "F.A.Q",
    icon: "mdi-frequently-asked-questions",
  },
  {
    title: "Videos",
    icon: "mdi-video",
  },
  {
    title: "Avisos",
    icon: "mdi-message-alert",
  },
];

export default defineComponent({
  name: "MainLayout",

  components: {
    EssentialLink,
  },

  setup() {
    const leftDrawerOpen = ref(false);
    const rightDrawerOpen = ref(false);

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },

      rightDrawerOpen,
      toggleRightDrawer() {
        rightDrawerOpen.value = !rightDrawerOpen.value;
      },
    };
  },
});
</script>
