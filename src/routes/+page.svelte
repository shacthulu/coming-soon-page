<svelte:head>
    <title>Exciting Updates Coming Soon</title>
	<meta name="description" content="We're working hard to bring you something amazing. Stay tuned for updates!" />
</svelte:head>

<div class="background">
	<div class="overlay">
		<div class="content">
			<h1>Something Exciting is Coming</h1>
			<p class="description">We're working hard to bring you something amazing. Stay tuned for updates!</p>
		</div>
	</div>
</div>

<style>
	:global(body) {
		font-family: 'Inter', sans-serif;
		margin: 0;
		padding: 0;
	}

	.background {
		background-image: url('/background.png');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
		min-height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.overlay {
		background-color: rgba(0, 0, 0, 0.5);
		width: 100%;
		height: 100%;
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 2rem;
	}

	.content {
		max-width: 60rem;
		text-align: center;
		color: white;
	}

	h1 {
		font-family: 'Inter', sans-serif;
		font-size: 2.5rem;
		font-weight: 700;
		margin-bottom: 8;
	}

	.description {
		font-size: 1rem;
		margin-bottom: 1.5rem;
		font-weight: 400;
	}

</style>
