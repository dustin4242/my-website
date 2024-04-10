<template>
	<div class="seperate">
		<div class="sidebar">
			Hello Welcome To My Website!
			------------
			<a href="/" class="button">Home</a>
			<a href="https://www.youtube.com/@DudeBroVideos" class="button">Youtube</a>
		</div>
		<a href="https://youtu.be/488YxXFIpz8">
			<NuxtImg src="/caprininha.gif" />
		</a>
	</div>
</template>

<style>
.seperate {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: space-between;
	min-width: 100px;
	width: 8%;
	height: 100%;
	padding-left: 5px;
	padding-right: 5px;
	background-color: #722f37;

	color: white;
	text-shadow: #19131e 2px 2px 2px;
	overflow-x: scroll;
}

.sidebar {
	display: flex;
	flex-direction: column;
	align-items: center;
	gap: 5px;
}

.button {
	color: white;
}

.end {
	width: 100%
}
</style>
