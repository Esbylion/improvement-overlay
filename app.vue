<template>
  <div>
    <NuxtRouteAnnouncer />
    test overlay edit
  </div>
</template>

<style>

  body {
    background-color: red;
  }

</style>

<script>
  addOverlayListener('CombatData', (data) => {
    console.log(`Encounter: ${data.title} | ${data.duration} | Total DPS: ${data.ENCDPS}`);
  });
</script>