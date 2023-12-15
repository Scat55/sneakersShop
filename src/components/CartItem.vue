<script setup lang="ts">
interface Props {
	imgUrl: string;
	text: string;
	price: number;
}

const props = defineProps<Props>();

const { imgUrl, price, text } = props;
</script>

<template>
	<div
		class="flex items-center w-full border border-slate-200 p-4 rounded-xl gap-4"
	>
		<img :src="imgUrl" alt="CardSneaker" class="w-16 h-16" />
		<div class="flex flex-col justify-between">
			<p>{{ text }}</p>
			<div class="flex justify-between mt-2">
				<b>{{ price }} руб.</b>
				<button class="opacity-40 hover:opacity-100 transition-all">
					<img src="/public/close.svg" alt="Close" />
				</button>
			</div>
		</div>
	</div>
</template>

<style scoped></style>
