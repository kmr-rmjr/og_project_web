<template>
<v-col lg="3" sm="4" cols="11">
  <v-card height="350" class="pa-3">
    <v-img
      :src="require('@/assets/img/' + ImgFile)"
      width="60%"
      class="mx-auto rounded-circle"
    ></v-img>
    <v-card-text class="text-lg-h6 font-weight-bold text-center mb-n6">{{Name}}</v-card-text>
    <v-card-text class="text-lg-subtitle-2 mb-n6">{{Position}}</v-card-text>
    <v-card-text class="text-lg-subtitle-2">{{Message}}</v-card-text>
  </v-card>
</v-col>
</template>

<script>
export default {
  props: {
    ImgFile: {
      type: String,
      required: true,
    },
    Name: {
      type: String,
      required: true,
    },
    Position: {
      type: String,
      required: true,
    },
    Message: {
      type: String,
      required: true,
    },
  }
}
</script>

<style>

</style>