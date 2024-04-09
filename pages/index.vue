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
	justify-content: center;
	align-items: center;
	width: 100%;
	background-color: #19161e;

	color: white;
	font-size: 2vw;
	text-shadow: #722f37 1px 1px 1px;
}

.window {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding: 15px;
	border-image-source: url("/window.png");
	border-image-outset: 15px;
	border-image-slice: 37 34 5;
	border-image-width: 37px 34px 5px 34px;
	border-image-repeat: round;
}
</style>
