<template>
<v-col lg="3" sm="4" cols="9" height="300px">
  <v-card flat height="100%" class="pa-3">
    <v-img
      :src="require('@/assets/img/members/' + imgFile)"
      :lazy-src="require('@/assets/img/members/' + imgFile)"
      width="60%"
      class="mx-auto rounded-circle"
    ></v-img>
    <v-card-text class="text-lg-h6 font-weight-bold text-center mb-n6">{{name}}</v-card-text>
    <v-card-text class="text-lg-subtitle-2 mb-n6">{{position}}</v-card-text>
    <v-card-text class="text-lg-subtitle-2">{{message}}</v-card-text>
  </v-card>
</v-col>
</template>

<script>
export default {
  props: {
    imgFile: {
      type: String,
      required: true,
    },
    name: {
      type: String,
      required: true,
    },
    position: {
      type: String,
      required: true,
    },
    message: {
      type: String,
      required: true,
    },
  }
}
</script>

<style>
</style>