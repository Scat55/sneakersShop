<script setup lang="ts">
interface Props {
	imgUrl: string;
	text: string;
	price: number;
	isFavorite: boolean;
	isAdded: boolean;
	changeFavorite: Function;
	changeAdded: Function;
}

const props = defineProps<Props>();
const { imgUrl, text, price, isFavorite, isAdded } = props;
</script>

<template>
	<div
		class="relative bg-white border border-slate-200 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
	>
		<button @click="changeFavorite">
			<img
				:src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
				alt="AddToFavorite"
				class="absolute top-8 left-8"
			/>
		</button>
		<img :src="imgUrl" alt="CardSneaker" />
		<p class="mt-2">{{ text }}</p>

		<div class="flex justify-between mt-5">
			<div class="flex flex-col">
				<span class="text-slate-400">Цена: </span>
				<b>{{ price }} руб. </b>
			</div>
			<button @click="changeAdded">
				<img :src="!isAdded ? '/plus.svg' : '/checked.svg'" alt="AddToCard" />
			</button>
		</div>
	</div>
</template>

<style scoped lang="scss"></style>
