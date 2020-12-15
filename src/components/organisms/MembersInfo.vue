<template>
  <v-row justify="center" justify-sm="start">
    <member-card
      v-for="member in membersInfo"
      :key="member.id"
      :img-file="`icon-member-${member.img}`"
      :name="member.name"
      :position="member.position"
      :message="member.message"
    ></member-card>
  </v-row>
</template>

<script>
import MemberCard from '@/components/molecules/MemberCard.vue'
import members from '@/assets/json/members_info.json';

export default {
  components: {
    MemberCard,
  },
  data() {
    return {
      membersInfo : members,
    }
  }
}
</script>