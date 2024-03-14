<script setup>
import WelcomeItem from './WelcomeItem.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
    </template>
    <template #heading>About</template>
    Allows for a proper elo system on the fly to ego other brothers on Pong.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
    </template>
    <template #heading>Leaderboard Page</template>
    This page ranks Brothers By Their ELO
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
    </template>
    <template #heading>Input</template>
    Use this page to input new scores into the system
    Input brothers names, winner, score won by, and if it was a sink or not
  </WelcomeItem>
</template>
