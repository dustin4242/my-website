<template>
	<div class="seperate">
		<div class="sidebar">
			<div>
				Hello Welcome To My Website!
				------------
			</div>
			<a href="/" class="button">Home</a>
			<a href="https://www.youtube.com/@DudeBroVideos" class="button">Youtube</a>
		</div>
		<div>
			<a href="https://youtu.be/488YxXFIpz8">
				<NuxtImg src="/caprininha.gif" />
			</a>
		</div>
	</div>
</template>

<style>
.sidebar {
	display: flex;
	flex-direction: column;
	align-items: center;
	gap: 5px;
}

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
}

.button {
	color: white;
}

.end {
	width: 100%
}
</style>
