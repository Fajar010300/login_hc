<template>
  <v-app>
    <div></div>
    <v-content>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center">
          <v-col cols="15" sm="10">
            <v-card class="elevation-2">
              <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" md="5">
                      <v-card-text class="mt-12">
                        <!-- <h1
                          class="text-center display-2 teal--text text--accent-2"
                        >
                          HOME CHARGING
                        </h1> -->

                        <!-- <div class="text-center mt-4">
                          <v-btn class="mx-2" fab color="black" outlined>
                            <v-icon>fab fa-facebook-f</v-icon>
                          </v-btn>
                          <v-btn class="mx-2" fab color="black" outlined>
                            <v-icon>fab fa-google-plus-g</v-icon>
                          </v-btn>

                          <v-btn class="mx-2" fab color="black" outlined>
                            <v-icon>fab fa-linkedin-in</v-icon>
                          </v-btn>
                        </div> -->

                        <h2 class="text-left mlt-4">LOGIN</h2>
                        <br />
                        <h4 class="text-left mlt-4">
                          Silahkan login terlebih dahulu ke aplikasi
                        </h4>
                        <v-form>
                          <v-text-field
                            label="Masukan Email"
                            name="Email"
                            prepend-icon="email"
                            type="text"
                            color="black"
                          />
                          <v-text-field
                            id="Password"
                            label="Kata Sandi"
                            name="Password"
                            prepend-icon="lock"
                            type="password"
                            color="black"
                          />
                          <div class="captcha-wrap"></div>

                          <v-text-field
                            id="captcha-code"
                            label="Enter captcha"
                            name="Password"
                            prepend-icon="refresh"
                            type="input"
                            color="black"
                          />
                        </v-form>
                        <h3 class="text-center mt-3">Lupa Kata Sandi</h3>
                      </v-card-text>
                      <div class="text-center mt-2">
                        <v-btn rounded color="blue" dark>Login</v-btn>
                      </div>
                    </v-col>
                    <v-col cols="12" md="8"></v-col>
                  </v-row>
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>
<script>
export default {
  data: () => ({
    step: 1,
  }),
  props: {
    source: String,
  },
};
</script>
