<template>
  <v-main>
    <!-- mv -->
    <v-container class="bg-linear height-100vh pt-10 pt-sm-0" fluid>
      <!-- header -->
      <template v-if="$vuetify.breakpoint.xs">
      </template>
        <template v-else>
          <v-app-bar
            dark
            color="rgb(0, 0, 0, 0)"
            flat
            class="mb-10"
          >
            <v-toolbar-title>2020 OGATA PROJECT</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-toolbar-items>
              <v-btn text @click="goto('#about')">About</v-btn>
              <v-btn text @click="goto('#activities')">Activities</v-btn>
              <v-btn text @click="goto('#products')">Products</v-btn>
              <v-btn text @click="goto('#members')">members</v-btn>
            </v-toolbar-items>
          </v-app-bar>
        </template>
      <!-- mv-content -->
      <h1 class="text-lg-h3 text-center white--text">OGATA PROJECT 2020</h1>
      <h2 class="text-lg-h5 text-center white--text font-weight-bold">AIにオノマトペの力を</h2>
      <v-row justify="center">
        <v-col lg="4" sm="8">
          <v-img contain max-height="100%" src="@/assets/img/img-robot.png"></v-img>
        </v-col>
      </v-row>
    </v-container>

    <!-- about -->
    <section id="about" class="bg-yellow">
      <v-container fluid>
        <v-row align="center" justify="center">
          <v-col cols="11" lg="5" sm="9">
            <h3 class="text-center text-h5 text-sm-h4 text-lg-left font-weight-bold mb-6">オノマトペという言葉を知る</h3>
            <p class="text-lg-subtitle-1">私達はオノマトペの持つ多彩な表現力に注目しました。ドキドキ、わくわく、ズキズキなど、私達はオノマトペという強力な表現を理解し、日常的に使用しています。しかし、このような表現は機械にとって非常に難解なものです。<br>
            私たち尾形プロジェクトの目標は、様々な方へのインタビューや検証を通じて言語学的側面からオノマトペという言葉を理解すること、機械翻訳と人知を組み合わせオノマトペの表現に特化したハイブリッド翻訳機を完成させることです。</p>
          </v-col>
          <v-col cols="11" lg="5" sm="7">
            <v-img src="@/assets/img/img-brain.png" max-width="100%"></v-img>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <!-- activities -->
    <section id="activities" class="bg-light-gray">
      <v-container fluid>
        <h2 :class="heading">Activities</h2>
          <activities></activities>
      </v-container>
    </section>

    <!-- products -->
    <section id="products" class="bg-salmon">
      <v-container fluid>
        <h2 :class="heading">Products</h2>
        <v-row justify="center">
          <v-col v-bind="contain">
            <products></products>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <!-- members -->
    <section id="members" class="bg-light-gray">
      <v-container fluid>
        <h2 :class="heading">Members</h2>
        <v-row justify="center">
          <v-col v-bind="contain">
            <members-info></members-info>

          </v-col>
        </v-row>
      </v-container>
    </section>
  </v-main>
</template>

<script>
import Activities from '../organisms/Activities.vue'
import MembersInfo from '../organisms/MembersInfo.vue'
import Products from '../organisms/Products.vue'
export default {
  components: {
    Activities,
    Products,
    MembersInfo,
  },
  data() {
    return {
      contain: {
        lg: 8,
      },
      heading: ["text-center", "text-h4", "text-lg-h3", "my-8", "font-weight-medium"]
    }
  },
  methods: {
    goto(destination) {
        this.$vuetify.goTo(destination);
    }
  }
}
</script>

<style>
.bg-linear {
  background: linear-gradient(#F9BAFE, #EFDDAE) !important;
}

.height-100vh {
  height: 100vh;
}

.bg-yellow {
  background-color: #EFDDAE;
}

.bg-salmon {
  background-color: #F3E3E3;
}

.bg-light-gray{
  background-color: #F6F6F6;
}
</style>