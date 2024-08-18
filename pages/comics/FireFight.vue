<template>
	<div class="something">
		<div class="window">
			<h1>Bring A Shield To A Fire Fight</h1>
			<div class="comics">
				<NuxtImg v-for="comicpage in comic" :src="comicpage" class="page-comic" loading="lazy" />
			</div>
		</div>
	</div>
</template>

<script setup>
const comic = [
	"placcid-lNAndXPpmDoFsY2xTBxxpEQEeY6Qpk.png",
	"placcid2-4ybCct9dfvKv12UR1LekDaMoDJn3ap.png",
	"placcid3-keRIYY6QJslFYzCQ01Mw4IcFRm4KDB.png",
	"placcid4-omNAQGm1ZnzXyB8EZFOsEVDeMrQlJq.png"
].map(x => { return "https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Comics/Bring%20A%20Shield%20To%20A%20Fire%20Fight/" + x });
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
