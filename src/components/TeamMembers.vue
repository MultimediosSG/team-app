<script setup>
import TeamMembersItem from '@/components/TeamMembersItem.vue'
defineProps({
    members: Array
})
</script>
<template>
    <div class="place-self-center flex flex-col gap-y-3">
    <table class="table-fixed border-spacing-2 border-separate">
      <thead>
        <th class="text-left px-6 py-2">Name</th>
        <th class="text-left px-6 py-2">Email</th>
        <th class="text-left px-6 py-2">Status</th>
      </thead>
      <tbody>
        <TeamMembersItem v-for="member in members" :key="member.id" :name="member.name" :email="member.email" :status="member.status"></TeamMembersItem>

       

      </tbody>
    </table>
    <p class="text-right text-gray-600 italic">There are no remaining team spots. Upgrade to add more.</p>
  </div>
</template>