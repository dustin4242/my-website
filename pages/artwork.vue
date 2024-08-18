<template>
	<div class="something">
		<div class="window">
			<h1>Artwork</h1>
			<div class="artworks">
				<NuxtImg v-for="artwork in art" :src="artwork" class="art" />
			</div>
		</div>
	</div>
</template>

<script setup>
import { ref } from 'vue';
const art = ref([
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/felicity-N8FPVgrMI05DX6ZxkhAx7EEAbWeYGM.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/marcy-T4ZPLcxYSSYGGyAxjior04ZLQ8aofx.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/blondegirl-7rhCyDCR4UNXo3sakwm5QJqxEjnilJ.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/albumcover-Omb4ARbjwZP6uzPwF1Nfyo0nr2DOGz.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/domino-pEm16vL5zw5NqkeTI70XM7JXkK4v1j.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/car-egMzxDyHoaywlJiU244QxUhB1dt2Cg.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/whisper%20stupid-CLXBq1ipPFTZJ0R26IN6UFvEvJzrMR.png",
	"https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/whisper%20listening-s1ZYOURTiutEZLySibON4k4HDrBm5X.jpg"
]);
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
