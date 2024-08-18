<template>
	<title>Dustin's Website</title>
	<meta content="Dustin's Website" property="og:title" />
	<meta content="A Place Where Dustin Does Things" property="og:description" />
	<meta content="https://chatplex.dev/#a" property="og:url" />
	<meta
		content="https://jje5kufjadbnucw7.public.blob.vercel-storage.com/General/caprininha-8QoqN4R7G3xWTeUZ0P3O3BZvpxXDrL.gif"
		property="og:image" />
	<meta content="#722f37" data-react-helmet="true" name="theme-color" />

	<div class="something">
		<div class="window">
			<h1>Hello, And Welcome To Dustin's Website!</h1>
			<div>This is just a mockup for my website, but I'll add more in the future.</div>
		</div>
	</div>
</template>

<style>
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
