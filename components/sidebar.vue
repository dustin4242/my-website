<template>
	<div class="seperate">
		<div class="sidebar">
			<div class="top" />
			Hello Welcome To My Website!
			<div class="divider" />
			<a href="/">Home</a>
			<a href="/comics">Comics</a>
			<a href="/artwork">Artwork</a>
			<a href="/blog">Blog</a>
			<a href="https://www.youtube.com/@DudeBroVideos">Youtube</a>
		</div>
		<a href="https://youtu.be/488YxXFIpz8">
			<NuxtImg
				src="https://jje5kufjadbnucw7.public.blob.vercel-storage.com/General/caprininha-8QoqN4R7G3xWTeUZ0P3O3BZvpxXDrL.gif"
				class="cap" loading="lazy" />
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
	text-shadow: #19131e 2px 2px;
	overflow-x: scroll;
	border-right: solid black 2px;
}

.sidebar {
	display: flex;
	flex-direction: column;
	align-items: center;
	gap: 5px;
}

.divider {
	border-top: dashed 2px;
	width: 100%
}

.cap {
	border: solid #19131e 2px;
	margin-bottom: 5px
}

.top {
	height: 2px;
}
</style>
