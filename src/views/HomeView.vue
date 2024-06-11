<script setup>
import TeamHeader from '@/components/TeamHeader.vue';
import TeamMembers from '@/components/TeamMembers.vue';
import TeamFooter from '@/components/TeamFooter.vue';
import team from '@/team.json'


</script>

<template>

  <TeamHeader :team="team"></TeamHeader>
  <TeamMembers :team="team"></TeamMembers>
  <TeamFooter :team="team"></TeamFooter>

</template>
