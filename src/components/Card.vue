<script setup lang="ts"></script>

<template>
	<div
		class="relative bg-white border border-slate-200 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
	>
		<button>
			<img
				src="/like-2.svg"
				alt="AddToFavorite"
				class="absolute top-8 left-8"
			/>
		</button>
		<img src="/sneakers/sneakers-1.jpg" alt="CardSneaker" />
		<p class="mt-2">Мужские Кроссовки Nike Blazer Mid Suede</p>

		<div class="flex justify-between mt-5">
			<div class="flex flex-col">
				<span class="text-slate-400">Цена: </span>
				<b>12 999 руб. </b>
			</div>
			<button>
				<img src="/plus.svg" alt="AddToCard" />
			</button>
		</div>
	</div>
</template>

<style scoped lang="scss"></style>
