<template>
	<div class="something">
		<div class="window">
			<h1>Celina Comic 1 (Unfinished)</h1>
			<div class="comics">
				<NuxtImg v-for="(comicpage, index) in comic" :src="comicpage" class=" page-comic" loading="lazy" />
			</div>
		</div>
	</div>
</template>

<script setup>
const comic = [
	"CelinaComic1_1-ZySaYiGXjiliiKQabbS21fh1j1UFv1.jpg",
	"CelinaComic1_2-Zs5nWXLMqdW82kkJ1CWzrZFjFI0Zr9.jpg"
].map(x => { return "https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Comics/Celina%20Comic%201/" + x });
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

.something {
	overflow-x: scroll;
	width: 100%;
	height: 100%;
	color: white;
}

.window {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	margin: 10px;
	padding: 25px;
	border-image-source: url("/window.png");
	border-image-slice: 37 34 5;
	border-image-width: 37px 34px 5px 34px;
}
</style>
