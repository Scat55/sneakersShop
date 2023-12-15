<script setup lang="ts">
import CartItem from './CartItem.vue';
</script>
<template>
	<div class="flex flex-col gap-4">
		<CartItem
			imgUrl="/public/sneakers/sneakers-1.jpg"
			:price="12999"
			text="Мужские Кроссовки Nike Blazer Mid Suede"
		/>
		<CartItem
			imgUrl="/public/sneakers/sneakers-1.jpg"
			:price="12999"
			text="Мужские Кроссовки Nike Blazer Mid Suede"
		/>
		<CartItem
			imgUrl="/public/sneakers/sneakers-1.jpg"
			:price="12999"
			text="Мужские Кроссовки Nike Blazer Mid Suede"
		/>
		<CartItem
			imgUrl="/public/sneakers/sneakers-1.jpg"
			:price="12999"
			text="Мужские Кроссовки Nike Blazer Mid Suede"
		/>
	</div>
</template>

<style scoped></style>
