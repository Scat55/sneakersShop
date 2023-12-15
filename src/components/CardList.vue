<script setup lang="ts">
import Card from '@/components/Card.vue';
</script>

<template>
	<div class="grid grid-cols-4 gap-5">
		<Card v-for="item in 5" />
	</div>
</template>

<style scoped lang="scss"></style>
