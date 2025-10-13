<script setup>
import JobListings from '@/components/JobListings.vue';
import Hero from '@/components/Hero.vue';
import HomeCards from '@/components/HomeCards.vue';
</script>

<template>
<Hero />
<HomeCards/>
<JobListings :limit="3" :show-button="true"/>
</template>