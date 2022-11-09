<template>
  <q-page class="q-pa-lg">
    <div class="row">
      <div class="col-4">
        <q-card class="q-mr-md" style="height: 300px">
          <q-card-section class="bg-teste text-white text-weight-bolder">
            <q-icon class="q-pr-sm" size="20px" name="mdi-comment-alert" />
            BEM VINDO
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card class="q-mr-md" style="height: 300px">
          <q-card-section class="bg-teste text-white text-weight-bolder">
            <q-icon class="q-pr-sm" size="20px" name="mdi-comment-alert" />
            PONTUAÇÃO
          </q-card-section>
          <q-card-section class="text-center">
            <div>
              <div class="text-h1 text-weight-bold q-mt-xl">
                60000 <spam class="text-h6 text-weight-bold">Pt</spam>
              </div>
            </div>
          </q-card-section>

          <!-- <img
            src="../../assets/kisspng-donuts-pie-chart-android-donut-creative-chart-5ad990a06947b7.3138264915242077764312.jpg"
          /> -->
        </q-card>
      </div>

      <div class="col-4">
        <q-card class="" style="height: 300px">
          <q-card-section class="bg-teste text-white text-weight-bolder">
            <q-icon class="q-pr-sm" size="20px" name="mdi-comment-alert" />
            POSIÇÃO
          </q-card-section>
          <q-card-section class="text-h1 text-weight-bold q-mt-xl text-center">
            <spam class="text-h4 text-weight-bold">#</spam> 32
          </q-card-section>
          <!-- <img
            src="../../assets/kisspng-donuts-pie-chart-android-donut-creative-chart-5ad990a06947b7.3138264915242077764312.jpg"
          /> -->
        </q-card>
      </div>
    </div>

    <div class="row q-pt-lg">
      <div class="col-6">
        <q-card>
          <q-card-section class="bg-teste text-white text-weight-bolder">
            <q-icon class="q-pr-sm" size="20px" name="mdi-comment-alert" />
            JOGOS
          </q-card-section>

          <q-markup-table>
            <thead>
              <tr>
                <th class="text-left">Jogos</th>
                <th class="text-right">Placar</th>
                <th class="text-right">Hora</th>
                <th class="text-right">Status</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td class="text-left">Brasil x Uruaguai</td>
                <td class="text-right">0 x 0</td>
                <td class="text-right">20:00</td>
                <td class="text-right">Aguardando</td>
              </tr>
              <tr>
                <td class="text-left">Espanha x Portugal</td>
                <td class="text-right">0 x 0</td>
                <td class="text-right">21:00</td>
                <td class="text-right">Aguardando</td>
              </tr>
              <tr>
                <td class="text-left">Italia x EUA</td>
                <td class="text-right">0 x 0</td>
                <td class="text-right">08:00</td>
                <td class="text-right">Aguardando</td>
              </tr>
              <tr>
                <td class="text-left">Holanda x Costa rica</td>
                <td class="text-right">0 x 0</td>
                <td class="text-right">10:00</td>
                <td class="text-right">Aguardando</td>
              </tr>
              <tr>
                <td class="text-left">Equador x Venezuela</td>
                <td class="text-right">0 x 0</td>
                <td class="text-right">14:00</td>
                <td class="text-right">Aguardando</td>
              </tr>
            </tbody>
          </q-markup-table>
        </q-card>
      </div>
      <div class="q-pl-md col-6">
        <q-card>
          <q-card-section class="bg-teste text-white text-weight-bolder">
            <q-icon class="q-pr-sm" size="20px" name="mdi-chart-line" />
            RANKING</q-card-section
          >

          <q-markup-table>
            <thead>
              <tr>
                <th class="text-left">Posição</th>
                <th>Usuario</th>
                <th>Pontuação</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td class="text-left">1</td>
                <td class="text-center">fulano</td>
                <td class="text-center">22</td>
              </tr>
              <tr>
                <td class="text-left">2</td>
                <td class="text-center">fulano</td>
                <td class="text-center">2</td>
              </tr>
              <tr>
                <td class="text-left">3</td>
                <td class="text-center">fulano</td>
                <td class="text-center">15</td>
              </tr>
              <tr>
                <td class="text-left">4</td>
                <td class="text-center">fulano</td>
                <td class="text-center">30</td>
              </tr>
              <tr>
                <td class="text-left">5</td>
                <td class="text-center">fulano</td>
                <td class="text-center">1</td>
              </tr>
            </tbody>
          </q-markup-table>
        </q-card>
      </div>
    </div>

    <!-- <div class="q-pt-md">
        <q-card>
          <q-card-section class="bg-teste text-white text-weight-bolder">
            <q-icon class="q-pr-sm" size="20px" name="mdi-room-service" />
            CHAMADOS
          </q-card-section>
          <q-markup-table>
            <thead>
              <tr>
                <th class="text-left">Titulo</th>
                <th class="text-right">Data/Hora</th>
                <th class="text-right">Data Fechamento</th>
                <th class="text-right">Status</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td class="text-left">Paula</td>
                <td class="text-right">22</td>
                <td class="text-right">3</td>
                <td class="text-right">22</td>
              </tr>
              <tr>
                <td class="text-left">Redacao</td>
                <td class="text-right">2</td>
                <td class="text-right">5</td>
                <td class="text-right">1</td>
              </tr>
              <tr>
                <td class="text-left">Jackeline Brazao</td>
                <td class="text-right">15</td>
                <td class="text-right">4</td>
                <td class="text-right">10</td>
              </tr>
              <tr>
                <td class="text-left">Juarez</td>
                <td class="text-right">30</td>
                <td class="text-right">10</td>
                <td class="text-right">15</td>
              </tr>
              <tr>
                <td class="text-left">Bruno</td>
                <td class="text-right">1</td>
                <td class="text-right">1</td>
                <td class="text-right">1</td>
              </tr>
            </tbody>
          </q-markup-table>
        </q-card>
      </div> -->
  </q-page>
</template>

<script>
export default {
  name: "DashBoard",
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
</style>
