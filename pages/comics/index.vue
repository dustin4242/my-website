<template>
	<div class="something">
		<div class="window">
			<h1>Comics</h1>
			<div class="comics">
				<a v-for="comic in comics" :href="/comics/ + comic[0]" class="link">{{ comic[1] }}</a>
			</div>
		</div>
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

.link {
	color: white;
	text-decoration: underline;
}
</style>
