<template>
	<h1>{{ comic.name }}</h1>
	<div class="comics">
		<NuxtImg v-for="(comicpage, index) in comic_pages" :src="comicpage" class=" page-comic" loading="lazy" />
	</div>
</template>

<script setup>
import comic_json from "../../public/art.json"
const route = useRoute();
const comic = comic_json.comics.find(x => x.routename == route.params.id)
const comic_pages = comic.pages.map(x => { return "https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Comics/" + comic.vercelname + "/" + x });
</script>

<style>
.comics {
	display: grid;
	grid-template-columns: auto auto;
	justify-content: center;
	column-gap: 5px;
	row-gap: 5px;
	height: 100%;
	width: 100%;
}

.page-comic {
	width: 100%;
	max-height: 80vh;
	object-fit: contain;
}
</style>
