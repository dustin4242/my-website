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
	text-shadow: #722f37 1px 1px 1px;
}

.window {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding: 15px;
	background-color: #211e26;
	border-image-source: url("/window.png");
	border-image-slice: 32 32 2;
	border-image-width: 32px 32px 2px 32px;
	border-image-repeat: round;
}
</style>
