<script setup lang="ts">
import { reactive } from 'vue';

interface Menu {
	img: string;
	text: string;
}

const menu: Menu[] = reactive([
	{
		img: '/cart.svg',
		text: '1205 руб.',
	},
	{
		img: '/heart.svg',
		text: 'Закладки',
	},
	{
		img: '/profile.svg',
		text: 'Профиль',
	},
]);
</script>

<template>
	<header class="flex justify-between border-b border-slate-300 px-10 py-8">
		<!--Logo-->
		<div class="flex items-center gap-4">
			<img src="/logo.png" alt="Logo" class="w-10" />
			<div>
				<h2 class="font-bold text-xl uppercase">Vue Sneakers</h2>
				<p class="text-slate-400">Магазин лучших кросовок</p>
			</div>
		</div>
		<ul class="flex items-center gap-10">
			<!--Menu-->
			<li
				class="flex items-center gap-3 text-gray-500 cursor-pointer hover:text-black"
				v-for="(item, idx) in menu"
				:key="idx"
			>
				<img :src="item.img" alt="Cart" />
				<span>{{ item.text }}</span>
			</li>
		</ul>
	</header>
</template>

<style scoped lang="scss"></style>
