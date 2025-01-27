<template>
	<h1>Artwork</h1>
	<div class="artworks">
		<NuxtImg v-for="artwork in art" :src="artwork" class="art" loading="lazy" />
	</div>
</template>

<script setup>
const img = useImage();
let art = [
	"sadness-0Nd9s81wm0uQuV6uJXx2AGvaZIsXj7.png",
	"theangelsmyth-OSNdzD5xoXWq4IRm8o9p21NJltthN0.png",
	"randomgirl-KXIATGc0BT6HXwv10eRtfQ7vjA7r5b.png",
	"celinadepressed-nTktfxUE5RVVswP8kIa2L90Mb1VyAT.png",
	"CelinaOHSHIT-PSAPPl8bQdr1ADTWgTxflkYRpYC8N7.png",
	"felicity-N8FPVgrMI05DX6ZxkhAx7EEAbWeYGM.png",
	"siris-bKAWz8M2rTTwsSw60msYmqfmjTh0Xk.png",
	"morbought-YARAt6B8hpsL6yLdlXT26mmg6g8zXy.png",
	"marcy-T4ZPLcxYSSYGGyAxjior04ZLQ8aofx.png",
	"blondegirl-7rhCyDCR4UNXo3sakwm5QJqxEjnilJ.png",
	"albumcover-Omb4ARbjwZP6uzPwF1Nfyo0nr2DOGz.png",
	"domino-pEm16vL5zw5NqkeTI70XM7JXkK4v1j.png",
	"car-egMzxDyHoaywlJiU244QxUhB1dt2Cg.png",
	"whisper%20stupid-CLXBq1ipPFTZJ0R26IN6UFvEvJzrMR.png",
	"whisper%20listening-s1ZYOURTiutEZLySibON4k4HDrBm5X.jpg"
].map(x => { return "https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Artwork/" + x });
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
