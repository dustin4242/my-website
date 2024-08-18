<template>
	<div class="page">
		<sidebar class="sidebar-shadow" />
		<div class="something">
			<div class="window">
				<NuxtPage />
			</div>
		</div>
	</div>
</template>

<style>
@font-face {
	font-family: 'Helvetica';
	src: url("/NbpInformaFivesix.ttf");
	font-weight: bolder;
	font-style: normal;
}

body,
#__nuxt {
	width: 100%;
	height: 100vh;
	margin: 0;
	font-family: 'Helvetica', monospace;
	font-size: 20pt;
	background-color: #19161e;
}

.page {
	display: flex;
	width: 100%;
	height: 100%;
}

a:link,
a:visited {
	color: white;
	text-decoration: underline;
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
