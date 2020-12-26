<template>
  <div>
    <product-info
      img-file="img-app-web.png"
      title="オノマトーク for Web"
    >
    <template v-slot:feature>
      <li class="mb-3">痛みのオノマトペを外国語で伝えることに特化したコミュニケーター</li>
      <li class="mb-3">様々な言語への翻訳に対応</li>
      <li class="mb-3">Web上で利用可能 (PC, スマートフォン, タブレット対応)</li>
    </template>
    <template v-slot:product-link>
      <v-btn href="https://onomatalk.web.app/" target="blank" color="#BB6BD9" class="white--text font-weight-bold mt-3 ml-5">オノマトークを試す</v-btn>
    </template>
    </product-info>

    <product-info
      img-file="img-app-ios.png"
      title="オノマトーク for Pythonista3"
    >
    <template v-slot:feature>
      <li class="mb-3">痛みのオノマトペを外国語で伝えることに特化したコミュニケーター</li>
      <li class="mb-3">様々な言語への翻訳に対応</li>
      <li class="mb-3">音声入力, 読み上げ機能搭載</li>
    </template>
    </product-info>

  </div>
</template>

<script>
import ProductInfo from '@/components/molecules/ProductInfo.vue'
export default {
  components: {
    ProductInfo,
  }
}
</script>

<style>

</style>