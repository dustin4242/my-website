<template>
	<div class="something">
		<div class="window">
			<h1>Hello, And Welcome To Dustin's Website!</h1>
			<div>This is just a mockup for my website, but I'll add more in the future.</div>
		</div>
	</div>
</template>

<style>
.something {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	overflow-x: scroll;
	width: 100%;
	background-color: #19161e;
	color: white;
}

.window {
	margin: 10px;
	padding: 25px;
	text-wrap: balance;
	border-image-source: url("/window.png");
	border-image-slice: 37 34 5;
	border-image-width: 37px 34px 5px 34px;
	text-shadow: #19161e 2px 2px;
}
</style>
