<template>
  <v-col lg="3" sm="7" cols="11">
    <v-card flat color="rgb(0, 0, 0, 0)">
      <v-img
        :src="require('@/assets/img/' + imgFile)"
        width="40%"
        class="mx-auto"
      ></v-img>
      <v-card-text
        class="text-lg-subtitle-1 font-weight-bold text-center mb-n6"
      >{{title}}</v-card-text>

      <v-card-text
        class="text-body-2"
      >{{text}}</v-card-text>
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
    title: {
      type: String,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },
  }
}
</script>

<style>

</style>