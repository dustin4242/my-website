<template>
	<h1>Comics</h1>
	<div class="comics">
		<a v-for="comic in comics" :href="/comics/ + comic[0]" class="link">{{ comic[1] }}</a>
	</div>
</template>

<script setup>
// Link Name, Full Name
const comics = [
	["CelinaComic1", "Celina Comic 1 (Unfinished)"],
	["FireFight", "Bring A Shield To A Fire Fight"]
];
</script>

<style>
.comics {
	display: flex;
	flex-direction: column;
	align-items: center;
	gap: 10px
}

.link {
	color: white;
	text-decoration: underline;
}
</style>
