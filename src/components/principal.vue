<template>
  <v-app>
    <div class="fondo-p" color="ffff">
      <div>
        <v-app-bar color="#131931" dense dark height="70">
          <router-link :to="{ name: 'inicio' }" class="noneline">
            <v-btn icon
              ><img
                src="https://i.ibb.co/7gyc5fX/maira.png"
                alt=""
                border="0"
                width="110px"
                height="75px"
              />
              <v-icon></v-icon>
            </v-btn>
          </router-link>
          <router-link :to="{ name: 'inicio' }" class="noneline">
            <h2 class="fuente" style="color: rgb(247, 252, 252)">
              Sistema financiero colombiano
            </h2>
          </router-link>
        </v-app-bar>
      </div>
      <div class="fondo-p">
        <v-parallax
          dark
          src="https://libreshot.com/wp-content/uploads/2016/02/business-861x528.jpg "
          height="625"
          class="fondo-p"
        >
          <v-container fluid>
            <v-row>
              <v-col cols="2">
                <v-row>
                  <v-card color="indigo darken-2" flat class="navbar">
                    <v-navigation-drawer
                      fluid
                      class="headline mb-1"
                      permanent
                      expand-on-hover
                      color="primary"
                      rounded
                      height="73"
                    >
                      <v-list-item dark fluid class="pa-0"
                        ><img
                          img
                          src="https://i.ibb.co/v16j4QV/nsasns.png"
                          alt="nsasns"
                          border="0"
                          rounded
                          width="61px"
                          height="70px"
                        />

                        <router-link
                          :to="{ name: 'contenido' }"
                          class="noneline"
                        >
                          <v-btn-fab
                            color="primary"
                            depressed
                            elevation="5"
                            icon
                            outlined
                            raised
                            tile
                            x-large
                            x-small
                            ><h3 style="color: rgb(247, 252, 252)">
                              Contenido
                            </h3></v-btn-fab
                          >
                        </router-link>
                      </v-list-item>
                    </v-navigation-drawer>
                  </v-card>
                </v-row>

                <v-row>
                  <v-card color="indigo darken-2" flat class="navbar">
                    <v-navigation-drawer
                      flat
                      fluid
                      class="headline mb-1"
                      permanent
                      expand-on-hover
                      color="primary"
                      height="73"
                    >
                      <v-list-item dark fluid class="pa-0" round
                        ><img
                          img
                          src="https://i.ibb.co/MSXKFpX/actividades.png"
                          alt="actividades"
                          border="0"
                          width="65px"
                          height="65px"
                        />

                        <router-link
                          :to="{ name: 'actividades' }"
                          class="noneline"
                        >
                          <v-btn-fab
                            color="primary"
                            elevation="5"
                            outlined
                            raised
                            rounded
                            text
                            x-large
                            x-small
                            ><h3 style="color: rgb(247, 252, 252)">
                              Actividades
                            </h3></v-btn-fab
                          >
                        </router-link>
                      </v-list-item>
                    </v-navigation-drawer>
                  </v-card>
                </v-row>

                <v-row>
                  <v-card color="indigo darken-2" flat>
                    <v-navigation-drawer
                      fluid
                      class="headline mb-1"
                      permanent
                      expand-on-hover
                      color="primary"
                      height="70"
                    >
                      <v-list-item dark fluid class="pa-0"
                        ><img
                          img
                          src="https://i.ibb.co/W5ZMzMR/eval.png"
                          alt="eval"
                          border="0"
                          width="60px"
                          height="65px"
                        />

                        <router-link
                          :to="{ name: 'evaluacion' }"
                          class="noneline"
                        >
                          <v-list-item-title
                            ><h2 style="color: rgb(247, 252, 252)">
                              Evaluacion
                            </h2></v-list-item-title
                          >
                        </router-link>
                      </v-list-item>
                    </v-navigation-drawer>
                  </v-card>
                </v-row>

                <v-row>
                  <v-card color="indigo darken-2" flat>
                    <v-navigation-drawer
                      fluid
                      class="headline mb-1"
                      permanent
                      expand-on-hover
                      color="primary"
                      height="73"
                    >
                      <v-list-item dark fluid class="pa-0"
                        ><img
                          src="https://i.ibb.co/4R67L4t/credittos.png"
                          alt="credittos"
                          border="0"
                          height="68px"
                          width="70px"
                        />

                        <router-link
                          :to="{ name: 'creditos' }"
                          class="noneline"
                        >
                          <v-btn-fab
                            color="primary"
                            elevation="5"
                            outlined
                            raised
                            rounded
                            text
                            x-large
                            x-small
                            ><h3 style="color: rgb(247, 252, 252)">
                              Creditos
                            </h3></v-btn-fab
                          >
                        </router-link>
                      </v-list-item>
                    </v-navigation-drawer>
                  </v-card>
                </v-row>
              </v-col>

              <v-row>
                <v-col aling="left" justific="center">
                  <v-main
                    color="rgb(255, 0, 0, 0.2)"
                    style="border: 0px solid powderblue"
                    class="fondo"
                    fixed
                  >
                    <router-view></router-view>
                  </v-main>
                </v-col>
              </v-row>
            </v-row>
          </v-container>
        </v-parallax>
      </div>
    </div>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
<style>
.fondo-p {
  height: 800px;
  background-color: rgb(7, 8, 31);
}
.degrade {
  background: radial-gradient(200px top, ellipse, white, #1162ac, black);
}

#alpha {
  background-color: rgba(200, 208, 231, 0.5);
  height: 2em;
  width: 150px;
  position: absolute;
  top: 10px;
  color: #fff;
  text-align: center;
  padding-top: 1em;
}
.fondo {
  background-color: rgba(0, 0, 0, 0.5);
  color: #fff;
  border-radius: 2rem;
}
</style>