<template>
  <v-row justify="center">
    <v-col cols="12" md="5" class="pr-0">
        <v-card height="640" color="transparent" elevation="4" class="rounded-r-0 rounded-xl text-center">
            <v-card-title>
              <v-btn fab icon color="transparent">
                <v-icon color="white">mdi-arrow-left</v-icon>
              </v-btn>
            </v-card-title>
            <v-col cols="12">
              <v-img :src="require('../assets/saas-logo.svg')" contain height="65"></v-img>
              <v-card-text class="pt-1 text-h5 font-weight-regular">Software</v-card-text>

              <v-card-text class="pt-0 pb-2 mt-6 text-h4 font-weight-bold">Welcome back</v-card-text>
              <v-card-text class="text-h6 py-0 font-weight-regular">Please login to continue</v-card-text>
            </v-col>
        </v-card>
    </v-col>

    <v-col cols="12" md="6" class="pl-0">
        <v-card height="640" color="white" elevation="4" class="rounded-l-0 rounded-xl pa-8">
            <v-row align="center" class="pb-4">
              <v-col cols="12" sm="4">
                <v-card-title class="black--text text-h4 pl-0 font-weight-bold">Login</v-card-title>
                <div class="purple-div mt-2"></div>
              </v-col>
              <v-spacer></v-spacer>
              <v-btn text rounded color="#9C27B0" class="text-caption">
                  <v-icon left small color="#9C27B0">mdi-arrow-right</v-icon> Create new account
              </v-btn>
            </v-row>
            <v-row align="center" class="d-flex justify-space-around mt-10 pb-4">
              <v-chip color="#3A559A" class="rounded-pill pl-7 pr-7 pb-5 pt-5 font-weight-bold text-uppercase">
                <v-icon left>mdi-facebook</v-icon>
                Facebook
              </v-chip>
              <v-chip color="#28AAE1" class="rounded-pill font-weight-bold text-uppercase pl-8 pr-8 pb-5 pt-5">
                <v-icon left>mdi-twitter</v-icon>
                Twitter
              </v-chip>
              <v-chip color="#DD493C" class="rounded-pill font-weight-bold text-uppercase pl-8 pr-8 pb-5 pt-5">
                <v-icon left>
                  mdi-google
                </v-icon>
                Google
              </v-chip>
            </v-row>

            <v-row align="center" justify="center" class="d-flex flex-row mt-10 pb-7">
              <div class="divider"></div>
              <p class="black--text text-subtitle-1 mb-0 px-6">Or login with email</p>
              <div class="divider"></div>
            </v-row>

            <v-form class="mt-8">
              <v-text-field solo outlined placeholder="Email" class="rounded-lg"></v-text-field>
              <v-text-field solo outlined placeholder="Password" type="password" class="rounded-lg"></v-text-field>

              <v-row align="center" class="px-4">
                <v-checkbox dark color="success"></v-checkbox>
                <p class="mb-0 grey--text">Remember me</p>
                <v-spacer></v-spacer>
                <p class="mb-0 purple--text text-subtitle-1">Forgot Password</p>
              </v-row>

              <v-btn block class="rounded-pill" color="success mt-4">Continue</v-btn>
            </v-form>
        </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {

}
</script>

<style>
.purple-div {
  content: "";
    width: 70px;
    height: 12px;
    border-radius: 12px;
    background: #9C27B0;
}

.divider {
  content: "";
    width: 70px;
    height: 1px;
    background: #CFCFCF;
}
</style>