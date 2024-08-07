<template>
	<div class="something">
		<div class="window">
			<h1>Blog</h1>
			<div>This is where my blog posts would go... if I had any.</div>
			<NuxtImg src="/dance.gif" class="dance" />
		</div>
	</div>
</template>

<style>
.dance {
	height: 300px;
}

.something {
	overflow-x: scroll;
	width: 100%;
	height: 100%;
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
