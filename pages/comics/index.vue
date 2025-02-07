<template>
	<h1>Comics</h1>
	<div class="comics">
		<a v-for="comic in comics" :href="/comics/ + comic.routename" class="link">{{ comic.name }}</a>
	</div>
</template>

<script setup>
// Link Name, Full Name
import comics_json from "../../public/art.json"
const comics = comics_json.comics;
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
