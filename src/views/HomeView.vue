<script setup>
import TeamHeader from '@/components/TeamHeader.vue';
import TeamMembers from '@/components/TeamMembers.vue';
import TeamFooter from '@/components/TeamFooter.vue';
import team from '@/team.json'


</script>

<template>

  <TeamHeader></TeamHeader>
  <TeamMembers :members="team"></TeamMembers>
  <TeamFooter></TeamFooter>

</template>
