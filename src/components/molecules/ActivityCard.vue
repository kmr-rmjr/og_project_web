<template>
  <v-col lg="3" sm="7" cols="11">
    <v-card flat>
      <v-img
        :src="require('@/assets/img/' + ImgFile)"
        width="40%"
        class="mx-auto"
      ></v-img>
      <v-card-text
        class="text-lg-subtitle-1 font-weight-bold text-center mb-n6"
      >{{Title}}</v-card-text>

      <v-card-text
        class="text-body-2"
      >{{Text}}</v-card-text>
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
    Title: {
      type: String,
      required: true,
    },
    Text: {
      type: String,
      required: true,
    },
  }
}
</script>

<style>

</style>