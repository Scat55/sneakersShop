<script setup lang="ts">
import Card from '@/components/Card.vue';

function changeFavorite() {
	alert('favorite');
}
function changeAdded() {
	alert(1);
}
</script>

<template>
	<div class="grid grid-cols-4 gap-5">
		<Card
			imgUrl="/sneakers/sneakers-1.jpg"
			:isFavorite="false"
			:price="12999"
			text="Мужские Кроссовки Nike Blazer Mid Suede"
			:isAdded="false"
			:changeFavorite="changeFavorite"
			:changeAdded="changeAdded"
		/>
	</div>
</template>

<style scoped lang="scss"></style>
