<template>
  <section id="contact" style="background: #3c4d5c">
    <v-container class="pt-10 mt-10">
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="10">
              <h1 class="display-2 font-weight-bold mb-4 mt-10 text-center white--text">
                Contacto
              </h1>
              <h1 class="font-weight-light mb-2 text-center white--text">
                Dime en que puedo ayudarte, y me pondre en contacto contigo
              </h1>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="10">
              <v-row align="center" justify="center">
                <v-col>
                  <v-img src="@/assets/contact me 2.svg" max-width="700"></v-img>
                </v-col>
                <v-col>
                  <v-form>
                    <v-row align="center" justify="center">
                      <v-col cols="12">
                        <v-text-field label="Nombre(s)" dark></v-text-field>
                      </v-col>
                      <v-col cols="12">
                        <v-text-field label="Primer apellido" dark></v-text-field>
                      </v-col>
                      <v-col cols="12">
                        <v-text-field label="Segundo apellido" dark></v-text-field>
                      </v-col>
                    </v-row>
                    <v-row align="center" justify="center">
                      <v-col>
                        <v-textarea label="Mensaje" rows="1" dark></v-textarea>
                      </v-col>
                    </v-row>
                    <v-row align="center" justify="center">
                      <v-col cols="4">
                        <v-btn x-large>
                          Enviar<v-icon right>mdi-send</v-icon>
                        </v-btn>
                      </v-col>
                    </v-row>

                  </v-form>
                </v-col>
              </v-row>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>