<template>
  <v-row justify="center" class="mb-12">
    <v-col lg="5" cols="11">
      <v-img
        :src="require('@/assets/img/' + imgFile)"
        width="40%"
        class="mx-auto"
      ></v-img>
    </v-col>

    <v-col class="mt-lg-14" lg="7" cols="11">
      <h3 class="text-lg-h5 font-weight-bold text-center text-lg-left mb-5">{{title}}</h3>
      <ul>
        <slot></slot>
      </ul>
    </v-col>
  </v-row>
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
  }
}
</script>

<style>

</style>