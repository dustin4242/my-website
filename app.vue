<template>
	<div class="page">
		<sidebar />
		<NuxtPage />
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
</style>
