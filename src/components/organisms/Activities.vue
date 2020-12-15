<template>
  <v-row justify="center">
    <activity-card
      img-file="icon-robot.svg"
      title="機械翻訳の抱える課題を解決"
      text="機械翻訳の苦手とする曖昧な表現における誤訳の解決に取り組んでいます。"
    ></activity-card>
    <activity-card
      img-file="icon-smartphone.svg"
      title="アプリケーション開発"
      text="機械翻訳と人知を組み合わせたハイブリッド翻訳アプリケーションを開発しています。"
    ></activity-card>
    <activity-card
      img-file="icon-conversation.svg"
      title="インタビュー"
      text="留学生や言語学に知見のある先生方へインビューを行い、言語学的な観点からオノマトペについて調査しています。"
    ></activity-card>
    </v-row>
</template>

<script>
import ActivityCard from '@/components/molecules/ActivityCard.vue';

export default {
  components: {
    ActivityCard,
  },
};
</script>
