<template>
	<h1>Artwork</h1>
	<div class="artworks">
		<NuxtImg v-for="artwork in art" :src="artwork" class="art" loading="lazy" />
	</div>
</template>

<script setup>
import art_json from "../public/art.json"
const img = useImage();
let art = art_json.art.map(x => { return "https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/" + x });
</script>

<style>
.artworks {
	display: grid;
	grid-template-columns: auto auto auto;
	justify-content: space-evenly;
	column-gap: 5px;
	row-gap: 5px;
	width: 100%;
	height: 100%
}

.art {
	max-height: 30vh;
	aspect-ratio: 1 / 1;
	object-fit: contain;
	width: 100%;
	background-color: #15121d;
}
</style>
