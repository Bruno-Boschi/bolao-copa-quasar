<template>
  <q-page class="q-pa-lg">
    <q-card class="q-pa-sm bg-teste" style="height: 50px">
      <div class="row text-white">
        <q-icon class="q-pa-xs" size="sm" name="mdi-page-next" />
        <div class="q-pl-md" style="font-size: 25px">Meus Palpites</div>
      </div>
    </q-card>

    <q-card class="q-mt-lg">
      <q-card>
        <q-tabs
          v-model="tab"
          dense
          class="text-grey"
          active-color="primary"
          indicator-color="primary"
          align="justify"
          narrow-indicator
        >
          <q-tab name="grupo" label="Fase de Grupo" />
          <q-tab name="eliminatoria" label="Eliminatoria" />
        </q-tabs>

        <q-separator />

        <q-tab-panels v-model="tab" animated>
          <q-tab-panel name="grupo" class="q-pa-sm">
            <div class="text-h6">Primeira etapa do Bolão Join Ads</div>
            <div class="q-mb-md">Faça seu Palpite.</div>

            <!--- Abetura --->
            <div class="row no-wrap">
              <div class="col-6 q-px-sm">
                <q-card flat bordered>
                  <q-card-section
                    class="row no-wrap items-center justify-center"
                  >
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/h0FNA5YxLzWChHS5K0o4gw_96x96.png"
                      />
                      CAT
                    </div>
                    <div class="row no-wrap items-center">
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                      <q-icon name="mdi-unfold-more-vertical" />
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                    </div>
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/AKqvkBpIyr-iLOK7Ig7-yQ_96x96.png"
                      />
                      EQU
                    </div>
                  </q-card-section>
                </q-card>
              </div>
            </div>
            <!--- Abetura  --->

            <!--- Inicio --->
            <div class="row no-wrap q-pt-md">
              <div class="col-6 q-px-sm">
                <q-card flat bordered>
                  <q-card-section
                    class="row no-wrap items-center justify-center"
                  >
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/DTqIL8Ba3KIuxGkpXw5ayA_96x96.png"
                      />
                      <div>ING</div>
                    </div>
                    <div class="row no-wrap items-center">
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                      <q-icon name="mdi-unfold-more-vertical" />
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                    </div>

                    <q-img
                      style="height: 50px; max-width: 50px"
                      src="https://ssl.gstatic.com/onebox/media/sports/logos/AKqvkBpIyr-iLOK7Ig7-yQ_96x96.png"
                    />
                    <div>IRA</div>
                  </q-card-section>
                </q-card>
              </div>

              <div class="col-6 q-px-sm">
                <q-card flat bordered>
                  <q-card-section
                    class="row no-wrap items-center justify-center"
                  >
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/zKLzoJVYz0bb6oAnPUdwWQ_96x96.png"
                      />
                      Brasil
                    </div>
                    <div class="row no-wrap items-center">
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                      <q-icon name="mdi-unfold-more-vertical" />
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                    </div>
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/AKqvkBpIyr-iLOK7Ig7-yQ_96x96.png"
                      />
                      Equador
                    </div>
                  </q-card-section>
                </q-card>
              </div>
            </div>

            <div class="row no-wrap q-pt-md">
              <div class="col-6 q-px-sm">
                <q-card flat bordered>
                  <q-card-section
                    class="row no-wrap items-center justify-center"
                  >
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/zKLzoJVYz0bb6oAnPUdwWQ_96x96.png"
                      />
                      Brasil
                    </div>
                    <div class="row no-wrap items-center">
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                      <q-icon name="mdi-unfold-more-vertical" />
                      <q-input
                        input-class="text-center"
                        style="max-width: 20px"
                        v-model="jogo1.time1"
                        placeholder="0"
                      />
                    </div>
                    <div class="q-mx-md">
                      <q-img
                        style="height: 50px; max-width: 50px"
                        src="https://ssl.gstatic.com/onebox/media/sports/logos/AKqvkBpIyr-iLOK7Ig7-yQ_96x96.png"
                      />
                      Equador
                    </div>
                  </q-card-section>
                </q-card>
              </div>
            </div>
            <!--- FIM  --->
          </q-tab-panel>

          <q-tab-panel name="eliminatoria">
            <div class="text-h6">Eliminatorias do Bolão Join</div>
            Fase elimitarória sera dividida em 4 etapas.
          </q-tab-panel>
        </q-tab-panels>
      </q-card>
    </q-card>
  </q-page>
</template>

<script>
import { ref } from "vue";

export default {
  name: "PalpitesPage",

  setup() {
    return {
      tab: ref("grupo"),
      jogo1: {
        time1: ref(""),
        time2: ref(""),
      },
    };
  },
};
</script>
