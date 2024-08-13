<template>
	<div class="something">
		<div class="window">
			<h1>Celina Comic 1</h1>
			<NuxtImg
				src="https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Comics/Celina%20Comic%201/CelinaComic1_1-LC6BX4HdzbelwTjllclXQ7e8ShEpaz.jpg"
				style="background-image: url(https://jje5kufjadbnucw7.public.blob.vercel-storage.com/Comics/Celina%20Comic%201/CelinaComic1_1_lowres-tkfYfBtlTWk9H79hgfCUX4RjZ0RzxL.jpg);"
				class="page-comic" />
		</div>
	</div>
</template>

<style>
.page-comic {
	max-height: 80vh;
	width: 100%;
	object-fit: contain;
	background-size: contain;
	background-position: center;
	background-repeat: no-repeat;
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
