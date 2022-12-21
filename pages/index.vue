<script lang="ts" setup>
const participants = [
  {
    name: "Jonas",
  },
  {
    name: "Roger",
  },
  {
    name: "Micha",
  },
  {
    name: "Jürgen",
  },
  {
    name: "Daniel",
  },
];
</script>

<template>
  <div>
    <MyTitle />
    <h1>Page: Index</h1>

    <ul>
      <li v-for="(participant, index) in participants" :key="index">
        <span :class="'tn-' + participant.name">{{ participant.name }}</span>
      </li>
    </ul>



  </div>
</template>

<style scoped></style>
