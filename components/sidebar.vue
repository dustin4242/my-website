<template>
	<div class="sidebar">
		<div>Hello Welcome To My Website!</div>
		<div>----------------------------</div>
		<a href="/" class="button">Home</a>
		<a href="https://www.youtube.com/@DudeBroVideos" class="button">Youtube</a>
	</div>
</template>

<style>
.sidebar {
	display: flex;
	flex-direction: column;
	align-items: center;
	min-width: 100px;
	width: 8%;
	height: 100%;
	gap: 5px;
	background-color: #722f37;

	color: white;
	padding-left: 5px;
	padding-right: 5px;
	text-shadow: #19131e 1px 1px 1px;
}

.button {
	color: white;
}

.end {
	width: 100%
}
</style>
